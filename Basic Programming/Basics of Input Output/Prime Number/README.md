# Solution

```
package main

import (
  "fmt"
  "math"
  )

func main(){
    var num int
    fmt.Scanf("%d",&num)

    for i:=2; i<num; i++{
      if(IsPrime(i)){
       fmt.Print(" ",i)
      }
    }
}


func IsPrime(value int) bool {
    for i := 2; i <= int(math.Floor(math.Sqrt(float64(value)))); i++ {
        if value%i == 0 {
            return false
        }
    }
    return true
}

```