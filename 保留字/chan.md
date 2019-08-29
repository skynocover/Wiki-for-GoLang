
## 宣告

``` go
chan T //可以用來發送與接收的通道

chan<-T //只能用來發送

<-chan T // 只能用來接收

```

----
## 初始化

``` go
ci := make(chan int)     //整数無緩衝

cj := make(chan int, 0)  //整数無緩衝

cp := make(chan *os.File, 100) //指向文件指標有緩衝

```
-----