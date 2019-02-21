# Package ddir

Package ddir provides functions for managing the application's data directory.

```go
import "github.com/godump/ddir"
```

- [Example](#Example)

# Example

`Base` sets base data path.

```go
ddir.Base("/tmp/play")
```

Create `/tmp/play/foo` if it doesn't exists.

```go
ddir.Make("foo")
```

Get absolute path `/tmp/play/bar` by given elems:

```go
name = ddir.Join("bar")
...
```
