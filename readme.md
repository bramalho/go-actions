# Go Actions

## Test

```bash
go test
go test -v
go test -cover
```

```bash
go test -cover -coverprofile=c.out
go tool cover -html=c.out -o coverage.html
```

## Lint

```bash
go env GOPATH GOBIN
```

in your bash source
```text
export GOPATH=$HOME/go
export GOBIN=$HOME/go/bin
```

```bash
go get -u golang.org/x/lint/golint
ls $GOBIN | grep golint
```

```bash
golint main.go
```
