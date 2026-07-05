# proto-gen-go

Generated Go bindings for the shared protobuf schemas defined in
[`altessa-s/proto`](https://github.com/altessa-s/proto). Do not edit
files in this repository by hand — they are regenerated and pushed
automatically on every push to `main` / `develop` and every `vX.Y.Z` tag.

## Install

```
go get github.com/altessa-s/proto-gen-go@latest
```

## Packages

| Import path | Source |
|-------------|--------|
| `github.com/altessa-s/proto-gen-go/io/altessa/badrequest/v1` | [`io/altessa/badrequest/v1`](io/altessa/badrequest/v1) |
| `github.com/altessa-s/proto-gen-go/io/altessa/serviceinfo/v1` | [`io/altessa/serviceinfo/v1`](io/altessa/serviceinfo/v1) |
| `github.com/altessa-s/proto-gen-go/io/altessa/type/v1` | [`io/altessa/type/v1`](io/altessa/type/v1) |

## Versioning

Versions are kept in lockstep with `altessa-s/proto` tags: a tag
`vX.Y.Z` on the schema repo yields the same tag here. The `main` and
`develop` branches track the corresponding schema branches; consumers
following `develop` use `go get @develop`.

## License

MIT — see [LICENSE](LICENSE).
