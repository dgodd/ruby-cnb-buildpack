# Sample Ruby Buildpack

To use this buildpack download `pack` from (github)[https://github.com/buildpack/pack/releases], then:

```
pack create-builder ruby-builder -b builder.toml
pack build <IMAGE NAME> --builder ruby-builder --path <RUBY APP PATH> --no-pull 
docker run -p 8080:8080 -e PORT=8080 <IMAGE NAME>
```
