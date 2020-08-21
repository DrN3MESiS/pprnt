# pprnt
Pretty Print for Golang (Maps, Models and Normal Variables)

## How to install

##### Version: 0.1.0
`go get github.com/DrN3MESiS/go-pprint`


## Description
Pretty Print is a Golang Package designed to print Maps and Structs as if they were JSON with Prettier  

### Usage
- Example Code:
```go
package main

import "github.com/DrN3MESiS/go-pprint"

func main(){
  example := map[string]interface{}{"get": map[string]interface{}{"some":"brother"}}
  
  // Print(interface) :: The function Print() expects an interface to be passed as parameters
  // So you can pass any type of variable
  pprint.Print(example) 
}
```
- Example Output
```
$ go run .

{
   "get": {
      "some": brother
   }
}
```

### Project Reason
Tired of printing structs or maps in go without any identation? Well, I was. I was tired of having to search for the key that I was looking for in the whole mess of the print. 
Imagine that you have a really big golang struct and you want to compare data between the same variable after some changes.
Without identation it would take a lot of effort to find the keys that you're looking for, and I was tired of that.

TL;DR: I hate printing structs or maps in go, and I created a solution.
