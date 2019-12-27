# Errors

## Concepts

Many programming languages allow `throwing` and `catching` errors, which allows developers to skip error handling in much of the function stack. Go strongly discurages this and instead guides programmers to use the `errors` package. This allows programmers to know exactly what inputs and outputs they have to deal with at the expense of verbosity.

```go
package main

import (
    "fmt"
    "errors"
)

func main() {
    val, err := doubleOrError(10)
    if err != nil {
        fmt.Println(err.Error())
    }
    fmt.Println("Success")

}

func doubleOrError(x int) (int, error) {
    if x % 2 == 0 {
        return 0, errors.New("x must be odd")
    }
    return x, nil
}
```

The important bits from this are:

`val, err := doubleOrError(10)`
- Val and err capture the return values of the function.

`if err != nil {`
- Handle the error appropriately if it exists.

`fmt.Println(err.Error())`
- `err.Error()` returns the string representation of the error.

`return 0, errors.New("x must be odd")`
- Even though we are returning an error, we must return all types declared in the function signature.
- `errors.New` creates a new error.

## Exercises

## Tips

## Further Reading

The source code if error is simple, go check it out!