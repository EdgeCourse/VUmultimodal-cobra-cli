# VUmultimodal-cobra-cli

About Cobra: https://pkg.go.dev/github.com/spf13/cobra

go get -u github.com/spf13/cobra@latest

go install -u github.com/spf13/cobra@latest

go run main.go -h

go run main.go reverse --help

# Invoke Reverse
go run main.go reverse foo
> oof

go run main.go rev bar
> rab

# Invoke Inspect
go run main.go inspect lorem
> 'lorem' has 5 chars

go run main.go insp FooBar
> 'FooBar' has 6 chars

# inspect a string for digits
go run main.go inspect A1B2C3 --digits
> 'A2B2C3' has 3 digits

go run main.go insp A1B2C3 -d
> 'A2B2C3' has 3 digits

# check command help
go run main.go inspect --help

Inspects a string

Usage:
  stringer inspect [flags]

Aliases:
  inspect, insp

Flags:
  -d, --digits   Count only digits
  -h, --help     help for inspect

