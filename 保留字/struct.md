```go
type Vertex struct {

X, Y int

}

var (

v1 = Vertex{1, 2} 宣告並給值

v2 = Vertex{X: 1} Y:0 被省略

v3 = Vertex{} X:0 和 Y:0

p = &Vertex{1, 2} 类型为 *Vertex

)
```