```go
var a interface{} //範用型別

//file接口
type File interface {

Read(b Buffer) bool

Write(b Buffer) bool

Close()

}
```