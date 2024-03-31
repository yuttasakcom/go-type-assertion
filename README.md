# Go Type Assertion

## Example
```go
package main

func main() {
	var result = "Go Type Assertion"
	display(result)

	var result2 = 100
	display(result2)
}

func display(a interface{}) {
	if s, ok := a.(string); ok {
		println(s)
		return
	}

	if i, ok := a.(int); ok {
		println(i)
		return
	}
}

```