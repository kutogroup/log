# goprint

GoLang log API
You can print any variables (string, struct, slice, map, ptr and more)

Example:

```go
package main

import (
	"github.com/MouseSun/log"
)

type TestStruct1 struct {
	Id    int32
	Value string
}

type TestStruct struct {
	Id    int32
	Value string
	St    TestStruct1
}

func main() {
	test := TestStruct{1, "hello struct", TestStruct1{2, "hello struct2"}}
	log.O("test tag", test)
}

```