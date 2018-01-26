# Things to do

[x] `go test` is very slow because `doTestsReference()` tests processing of every substring of original markdown. Remove that and add a separate test program for that to be run only in CI

[x] instead of using NodeType, use interface{} for Node data, like xml parser

[x] simplify oliPrefix()

[ ] speed: Node is probably too fat

[ ] speed: Node could be allocated from a slice and pointers could be replaces with int32 integers. Node would have to keep track of the allocator or we can change the api to pass both Parser (which is allocator of nodes) and Node (which would be a typedef for int)

[ ] fuzzing!

[ ] SoftbreakData is not used