# Introduction:
  GoInfo is get os platform information coding by Golang.
  
  It can help you to know os information.
  
  
## Version:

version:0.1.0

## Futures

get linux information

get windows information

get osx information

get freebsd information
  
  
## Install:
```sh
  go get github.com/matishsiao/goInfo
  go build
```

## Struct:
```go
  type GoInfoObject struct {
	GoOS string
	Kernel string
	Core string
	Platform string
	OS string
	Hostname string
	CPUs int
}
```

## Example:

```go   
   package main

   import (
	   "github.com/julienlevasseur/goInfo"
   )

   func main() {
		gi := goInfo.GetInfo()
		gi.VarDump()
	 }
}
```

It's will show:

```
   GoOS: linux
   Kernel: Linux
   Core: 3.13.0-27-generic
   Platform: x86_64
   OS: GNU/Linux
   Hostname: ubuntu
   CPUs: 1
```

##License and Copyright
This software is Copyright 2012-2014 Matis Hsiao.
Copyright 2024 Julien Levasseur.
