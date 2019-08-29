```go
 const pi float64 = 3.14 
 ```

>表示在程式運行中不會被修改  
可以使用  
len(),cap(),unsafe(),sizeof()計算
```go

a="abc"

b=len(a)

iota //每有一行常量聲明就將iota+1

//(可將iota視為const中的索引)

const(
    a=iota  0
    b  1
    c  2
    d="ga" ga
    e ga
    f=100 100
    h=iota 6
)
 ```