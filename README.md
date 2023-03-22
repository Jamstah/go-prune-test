# go-prune-test

Test that importing a specific package from a module doesn't drag in dependencies that are not needed for that package.

Validation:
```
jammy:go$ go mod tidy
jammy:go$ go mod vendor
jammy:go$ go build ./...
```
