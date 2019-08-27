

----------

- 編譯
  - windows
    - GOOS=windows GOARCH=386 go build -o hello.exe hello.go
  - linux
    - GOOS=linux GOARCH=amd64 CGO_ENABLED=0 go build -o hello.go
  - maxOs
    - GOOS=darwin GOARCH=amd64 CGO_ENABLED=0 go build -o hello.go
------------------

- Package的使用
  - 將套件抓入src
    - go get github.com/syhlion/simplenum
  - 呼叫
    - simplenum.Round
    - simplenum表示package的名稱,而不是GO文件的名稱
    - Round的第一個字要大寫,不然沒辦法呼叫

-------------

- 常用操作
  - 字串長度
    - 使用 bytes.Count() 統計
    - 使用 strings.Count() 統計
    - 将字符串轉換為 []rune 後使用 len 函數進行統計
    - 使用utf8.RuneCountInString() 統計

    - >str:="HelloWord"

    - >l1:=len([]rune(str))
      l2:=bytes.Count([]byte(str),nil)-1)
      l3:=strings.Count(str,"")-1
      l4:=utf8.RuneCountInString(str)

      > 結果都是9
  - 指令
    - go env 
      > 可以看目前的環境變量


-------------

- 函數
  - strings
  - time
  - os
  - strconv
  - net/http
  - io/ioutil
  - fmt
--------------

- 保留字
  - 包管理
    - import
    - package
  - 聲明定義
    - chan
    - const
    - func
    - interface
    - map
    -  struct 
    - type
    - var
  - 流程控制
    - switch類
      - case
      - default
      - switch
      - fallthrough
    - 中斷類
      - continue
      - break
    - 其他
      - defer 
      - else
      - for
      - go
      - goto
      - if
      - range
      - return
      - select
      -chan
 