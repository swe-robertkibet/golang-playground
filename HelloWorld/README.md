### 1. ** Program Structure**

Here is the Hello World small program we created...

```go
package main

import "fmt"

func main() {
    fmt.Println("hello world")
}
```

#### Key Components :

1. **`package main`**:

   - Every Go program is part of a package. A package is a way to group related Go files together.
   - `main` is a special package name in Go. Programs that are meant to be executable must have a `main` package. The `main` package must also have a `main` function; this is the entry point of the program where execution begins.

2. **`import "fmt"`**:

   - `import` is used to include other packages that our program will use.
   - `"fmt"` is a package in the Go standard library that provides formatted I/O (input/output) functions.
   - In this case, we are using the `fmt` package to print output to the console.

3. **`func main()`**:

   - This is the main function where the execution of our Go program starts.
   - Every Go program must have a `main` function inside the `main` package. It’s the entry point of the executable program.

4. **`fmt.Println("hello world")`**:
   - `fmt.Println` is a function from the `fmt` package that prints the string provided to the console, followed by a newline.
   - `"hello world"` is the string literal being printed.

### 2. **Running the Program**

To run the Go program, we have a few steps to follow:

1. **Save the Program**:

   - Save the code in a file named `main.go`.

2. **Run the Program**:

   - Open our terminal or command prompt.
   - Navigate to the directory where we saved `main.go`.
   - Use the `go run` command to compile and run the program in one step:

   ```bash
   $ go run main.go
   ```

   - Output:

     ```
     hello world
     ```

   - `go run` compiles the Go source code and immediately runs it. This is convenient for quickly running and testing small programs.

3. **Building a Binary**:

   - To create an executable binary file of our program, we use the `go build` command:

   ```bash
   $ go build main.go
   ```

   - This command compiles the source code and produces a binary executable file named `main` (or `main.exe` on Windows).

4. **Execute the Binary**:

   - After building, we can execute the binary directly from the terminal:

   ```bash
   $ ./hello-world
   ```

   - Output:
     ```
     hello world
     ```

![Files and commands](./Screenshot%202024-09-03%20225637.png)

### 3. **Why Build a Binary?**

Building a binary allows us to:

- **Distribute**: Share the executable with others without requiring them to have Go installed.
- **Performance**: The binary is already compiled, so it runs faster than using `go run`, which compiles each time.
- **Portability**: The compiled binary can be run on any machine of the same architecture and OS without needing the Go source code.

### 3. **Commands used**

- **go run**
- **go build**
