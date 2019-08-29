> 宣告 string表鍵的型態 int表值的型態
```go
b := map[string]int { 
"s": 1, 
"b": 2, 
}
fmt.Println(b)
```

## 用法  
```go
nameAge := make(map[string]int)
```
### 增
``` go
nameAge["bob"] = 18

nameAge["tom"] = 16
```
### 删
``` go
delete(nameAge, "bob")
```
### 改
``` go
nameAge["tom"] = 19
```
### 查
``` go
v := nameAge["tom"]

fmt.Println("v=",v)
```
### 推荐查法
``` go
v, ok := nameAge["tom"]

if ok {

fmt.Println("v=",v,"ok=",ok)

}
```
### 遍歷
``` go
for k, v :=range nameAge {

fmt.Println(k, v)

}
```