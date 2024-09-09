# Go Constants

In Go, constants are fixed values that cannot be altered during the execution of a program. They are defined using the `const` keyword and can be of types such as `string`, `boolean`, `character`, and numeric types.

## Key Concepts

- **Immutability**: Once defined, the value of a constant cannot be changed.
- **Types**: Constants can hold values of several types, including strings, booleans, characters, and numbers.
- **Precision**: Go allows for arithmetic operations with constants to be performed with arbitrary precision.
- **Type Inference**: Numeric constants in Go are typeless until they are explicitly cast or used in a context that requires a specific type.

## Example

```go
package main

import (
    "fmt"
    "math"
)

const s string = "constant"

func main() {
    fmt.Println(s)

    const n = 500000000
    const d = 3e20 / n

    fmt.Println(d)
    fmt.Println(int64(d))
    fmt.Println(math.Sin(n))
}
```

# Output

![Screenshot of Go Constants Output](./Screenshot%202024-09-09%20203553.png)
