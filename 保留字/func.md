返回兩字串
```go
func swap(x, y string)(string, string)
 { return y, x }
```

可以在輸出的時候命名
```go
func swap2(sum float64)(x, y float64) 
{ x = sum / 2 y = sum * 2 return }
```
可以在輸出的時候命名
```go
func swap3(sum float64) (x, y float64) 
{ x = sum / 2 
y = sum * 2 
return x * 2, y / 2 }
```