# proto-gen-go

Generated Go bindings for the
[altessa-s/proto](https://github.com/altessa-s/proto) schema.

This repository is auto-generated. Do not edit its files by hand — they are
regenerated from [`altessa-s/proto`](https://github.com/altessa-s/proto) and
pushed automatically on every push to `main` / `develop` and every `vX.Y.Z`
tag. The only hand-maintained file is this `README.md`.

## Installation

```
go get github.com/altessa-s/proto-gen-go@latest
```

Consumers tracking the `develop` branch can use
`go get github.com/altessa-s/proto-gen-go@develop`.

## Packages

| Proto package | Import path | Description |
|---|---|---|
| `io.altessa.badrequest.v1` | `github.com/altessa-s/proto-gen-go/io/altessa/badrequest/v1` | `BadRequest` / `FieldViolation` error-detail payload for a `google.rpc.Status` with `INVALID_ARGUMENT`. |
| `io.altessa.serviceinfo.v1` | `github.com/altessa-s/proto-gen-go/io/altessa/serviceinfo/v1` | `ServiceInfo` runtime metadata plus the `ServiceInfoService.GetServiceInfo` introspection RPC. |
| `io.altessa.type.v1` | `github.com/altessa-s/proto-gen-go/io/altessa/type/v1` | General-purpose, domain-neutral value types (`Contact`, `DatePeriod`, `FileRef`, …) reused across services. |

## Usage

```go
import (
    serviceinfov1 "github.com/altessa-s/proto-gen-go/io/altessa/serviceinfo/v1"
)

info := &serviceinfov1.ServiceInfo{
    ServiceName: "billing-api",
    FullVersion: "1.4.2+build.873",
}
```

The gRPC service is `ServiceInfoService` with a single
`GetServiceInfo(GetServiceInfoRequest) returns (GetServiceInfoResponse)` RPC;
register a server implementation with
`serviceinfov1.RegisterServiceInfoServiceServer`.

## Versioning

Versions track [`altessa-s/proto`](https://github.com/altessa-s/proto): a
`vX.Y.Z` tag on the schema repo produces the same release here, and the
`main` / `develop` branches follow the matching schema branches.

## Contributing

This repository contains generated output only. To change what appears here,
edit the schemas or generation config in
[`altessa-s/proto`](https://github.com/altessa-s/proto); the next sync
regenerates and republishes these bindings.

## License

MIT — see [LICENSE](LICENSE).
