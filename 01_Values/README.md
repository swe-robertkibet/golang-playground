# Go Values

This is a basic Go program demonstrating the usage of different value types in Go, including strings, integers, floats, and booleans. The program prints various outputs to the console to show how these value types work.

## Code

```go
package main

import "fmt"

func main() {

    fmt.Println("go" + "lang")

    fmt.Println("1+1 =", 1+1)
    fmt.Println("7.0/3.0 =", 7.0/3.0)

    fmt.Println(true && false)
    fmt.Println(true || false)
    fmt.Println(!true)
}
```

## How to Run

1. Save the code in a file named `main.go`.

2. Open a terminal and navigate to the directory where `main.go` is saved.

3. Run the program using the following command:

   ```bash
   go run main.go
   ```

4. You should see the following output:

   ```
   golang
   1+1 = 2
   7.0/3.0 = 2.3333333333333335
   false
   true
   false
   ```

![Screenshot of Go Values Program Output](./Screenshot%202024-09-04%20202533.png)

## Explanation

- **Strings**: The program demonstrates string concatenation using the `+` operator.
- **Integers**: It shows basic integer arithmetic.
- **Floats**: It includes an example of floating-point division.
- **Booleans**: The program uses boolean operators like `&&`, `||`, and `!` to demonstrate logical operations.
