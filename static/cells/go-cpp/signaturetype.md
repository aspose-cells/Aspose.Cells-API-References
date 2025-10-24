##SignatureType Enum
'SignatureType enum. Encapsulates the object that represents signaturetype in Go.'
## SignatureType Enum
Specifies the signature type.
```go
type SignatureType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Default](./default/) | The default value , the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. |
|[Stamp](./stamp/) | The corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. |
|[Custom](./custom/) | The corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
