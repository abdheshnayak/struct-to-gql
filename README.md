# struct to gql

copied from [https://github.com/kloudlite/api/cmd/struct-to-graphql](https://github.com/kloudlite/api)

## Usage Guide

```bash
working_dir=$(mktemp -d)

mkdir -p "$working_dir"
- go run github.com/abdheshnayak/struct-to-gql
    --struct package.Entity # example: github.com/abdheshnayak/gorm-practice/app/entities.Todo
> $working_dir/main.go
- |+
pushd "$working_dir"
go run main.go --dev --out-dir ../graph/struct-to-graphql 
popd
- rm -rf $working_dir
```
