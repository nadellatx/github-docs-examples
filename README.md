# Writing good documentation

## Step 1 - Using code blocks

Codeblocks in markdown makes it *very easy* for tech people to **copy, paste, and share** code. A good _Cloud Engineer_ uses Codeblocks when possible.

```go

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
- Use code block for both code and errors that appear in console

```bash
Traceback(most recent call last):
 2: from /usr/bin/irb:23:in '<main>'
 1: from (irb):1
RuntimeError: This is a custom error message
```

## References
- [Github Flavored Markdown Spec](https://github.github.com/gfm/).
- [Github writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-formatting-syntax#quoting-text).


