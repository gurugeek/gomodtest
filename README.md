# gomodtest

Example showing module with different from GOPATH import name

## TL;DR
```sh
export GO111MODULE=on
go run main.go
```

## How it works?

`go.mod` files contains module name, which is different from package path. This is 100% correct for go modules.

One may safely import path-independent modules, as go ecosystem knows that the root of module is actually `github.com/example/gomodtest`, but not a `github.com/kchugalinskiy/gomodtest`
