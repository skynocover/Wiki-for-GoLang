一般的switch
```go
func choose(i int) { 
    switch i { 
        case 1: 
            fmt.Println("1") //不用break  
        case 2, 3: 
            fmt.Println("2or3") 
        case 4: 
            fallthrough //會跳到下一個case繼續判斷 
        case 5: fmt.Println("5") }

}
```
可以不用在switch寫陳述
```go
func choose2(i int) { 
    var jj = 0 s
    witch { 
        case i > 5: 
            fmt.Println(i, ">5") 
        case i < 5: 
            fmt.Println(i, "<5") 
        case jj == 0: 
            fmt.Println("i==5 , jj==0"
        //其餘的:使用default    
        } 

}


```