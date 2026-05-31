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
| `github.com/altessa-s/proto-gen-go/services/badrequest/v1` | [`services/badrequest/v1`](services/badrequest/v1) |
| `github.com/altessa-s/proto-gen-go/services/serviceinfo/v1` | [`services/serviceinfo/v1`](services/serviceinfo/v1) |
| `github.com/altessa-s/proto-gen-go/type/v1` | [`type/v1`](type/v1) |

## Versioning

Versions are kept in lockstep with `altessa-s/proto` tags: a tag
`vX.Y.Z` on the schema repo yields the same tag here. The `main` and
`develop` branches track the corresponding schema branches; consumers
following `develop` use `go get @develop`.

## License

MIT — see [LICENSE](LICENSE).
