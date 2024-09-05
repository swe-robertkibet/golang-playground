# Variables

In Go, variables must be explicitly declared, which helps the compiler ensure type correctness during function calls and other operations. Let's break down how we handle variables in Go, along with an explanation of the code above.

## 1. **Variable Declaration in Go**

We can declare variables in Go using the `var` keyword or using shorthand syntax (`:=`), depending on the context.

## 2. **Our Code Above**

Here's our code demonstrating variable declaration:

```go
package main

import "fmt"

func main() {
    // Declare a variable with initialization
    var a = "initial"
    fmt.Println(a)

    // Declare multiple variables at once
    var b, c int = 1, 2
    fmt.Println(b, c)

    // Go infers the type of initialized variables
    var d = true
    fmt.Println(d)

    // Variables declared without initialization are zero-valued
    var e int
    fmt.Println(e)

    // Shorthand syntax for declaring and initializing a variable
    f := "apple"
    fmt.Println(f)
}
```

## 3. **Output Screenshot**

![Screenshot of Variable Declaration Output](./Screenshot%202024-09-05%20202902.png)

## 4. **Explanation of our Code**

1. **Variable Declaration with Initialization**:

   - The `var` keyword is used to declare variables, and Go can infer the type of the variable from the assigned value.
   - Example:
     ```go
     var a = "initial"
     fmt.Println(a)
     ```
   - Output:
     ```
     initial
     ```

2. **Multiple Variable Declaration**:

   - We can declare multiple variables of the same type in one line.
   - Example:
     ```go
     var b, c int = 1, 2
     fmt.Println(b, c)
     ```
   - Output:
     ```
     1 2
     ```

3. **Type Inference**:

   - Go automatically infers the type of variables based on the value assigned, so we don't need to explicitly mention the type if it's obvious.
   - Example:
     ```go
     var d = true
     fmt.Println(d)
     ```
   - Output:
     ```
     true
     ```

4. **Zero-Valued Variables**:

   - Variables that are declared without an initial value are automatically assigned the **zero value** for their type.
   - For example, the zero value for an `int` is `0`.
   - Example:
     ```go
     var e int
     fmt.Println(e)
     ```
   - Output:
     ```
     0
     ```

5. **Shorthand Declaration and Initialization (`:=`)**:
   - Inside functions, Go allows the shorthand syntax `:=` for declaring and initializing variables in one line.
   - This is a more concise form of `var` declaration and is available only inside function bodies.
   - Example:
     ```go
     f := "apple"
     fmt.Println(f)
     ```
   - Output:
     ```
     apple
     ```

## 5. **Running the Code**

1. **Save the code** in a file named `main.go`.
2. **Run the code** in your terminal:

   ```bash
   $ go run variables.go
   ```

3. **Expected Output**:
   ```
   initial
   1 2
   true
   0
   apple
   ```

## 6. **Summary**

- **`var` keyword**: Used to declare variables. Go can infer the type from the value assigned.
- **Zero values**: Variables that are declared but not initialized are assigned a default zero value (e.g., `0` for integers, `false` for booleans).
- **Shorthand `:=`**: A more concise way to declare and initialize a variable, available only inside functions.
- **Type safety**: Go's explicit declarations help ensure type correctness during function calls and operations.
