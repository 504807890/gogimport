## gogimport
golang grouping import tool

### introduction

gogimport will grouping imports by stdlib, thirdparty, custom packages like the example below:

```sh
$ gogimport -local github.com/wusendong/example main.go
```

```go
package main

import (
    "fmt"
    "log"

    "gopkg.in/redis.v5"
    "github.com/gorilla/context"

    "github.com/wusendong/example"
)

```


### install
```
go get -u github.com/wusendong/gogimport
```


### usage
```
Usage of gogimport:
gogimport [options] [file ...]

Options:
  -local string
        local package name
Example command:
gogimport -local ${packaname} some.go other.go
```
