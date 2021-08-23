# golang 面试题总结

https://blog.csdn.net/weiyuefei/article/details/77963810

1. defer与panic

defer执行顺序是先进后出类似栈，panic 会等待之前的defer执行完成侯才会触发。

```go

func calc(index string, a, b int) int {
    ret := a + b
    fmt.Println(index, a, b, ret)
    return ret
}
 
func main() {
    a := 1
    b := 2
    defer calc("1", a, calc("10", a, b)) 
    a = 0
    defer calc("2", a, calc("20", a, b))
    b = 1
}
//  calc("10", a, b) 作为参数会最先执行
//  calc("20", a, b) 作为参数会先执行
//  calc("2", a, calc("20", a, b)) 执行顺序先会执行
//  calc("1", a, calc("10", a, b)) 最后执行
```



2. for 循环易错点

   ```go
   for(index,value: range array){
   	xxx[index] = &value
   }
   
   // xxx[index] 最终都指向最后一个元素的地址。
   ```

   ```go
    for i := 0; i < 10; i++ {
       go func(i int) { 
          
       }(i) 
    }
   
   // 如果i不以参数传递，闭包的函数获取到的i值始终未10。
   ```

3.  select三点原则

- select 中只要有一个case能return，则立刻执行。
- 当如果同一时间有多个case均能return则伪随机方式抽取任意一个执行。
- 如果没有一个case能return则可以执行”default”块

4. slice

   ```go
   s := make([]int, 5) // make([]int,0) or make([]int,0,5)
   s = append(s, 1, 2, 3)
   fmt.Println(s) // 0 0 0 0 0 1 2 3
   
   ```

   
