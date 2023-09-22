# Writing good documentation

## Step 1 - Using code blocks

Codeblocks in markdown makes it *very easy* for tech people to **copy, paste, and share** code. A good _Cloud Engineer_ uses Codeblocks when possible.

```
// This program defines a factorial function that calculates the factorial of a non-negative integer using recursion.
//It takes user input for a number and then calculates and prints its factorial. If the input is negative, it
//informs the user that factorial is not defined for negative numbers.

package main

import "fmt"

// Recursive function to calculate the factorial of a number
func factorial(n int) int {
    if n == 0 {
        return 1
    }
    return n * factorial(n-1)
}

func main() {
    var num int
    fmt.Print("Enter a number: ")
    fmt.Scan(&num)

    if num < 0 {
        fmt.Println("Factorial is not defined for negative numbers.")
    } else {
        result := factorial(num)
        fmt.Printf("The factorial of %d is %d\n", num, result)
    }
}

```




