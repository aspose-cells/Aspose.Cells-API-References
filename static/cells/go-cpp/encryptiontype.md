##EncryptionType Enum
'EncryptionType enum. Encapsulates the object that represents encryptiontype in Go.'
## EncryptionType Enum
Encryption Type.Only used by excel2003.We will encrypt 2007/2010 workbook using SHA AES the same as Excel does, and this EncryptionType will be ignored.
```go
type EncryptionType int32
```
## Fields
| Field | Description |
| --- | --- |
|[XOR](./xor/) | XOR encryption algorithm. |
|[Compatible](./compatible/) | Office 97/2000 compatible. |
|[EnhancedCryptographicProviderV1](./enhancedcryptographicproviderv1/) | Enhanced encryption. |
|[StrongCryptographicProvider](./strongcryptographicprovider/) | Strong encryption algorithm. |
