---
title: EncryptionType Enum 
linktitle: EncryptionType
second_title: Aspose.Cells for Go API Reference
description: 'EncryptionType enum. Encapsulates the object that represents encryptiontype in Go.'
type: docs
weight: 200
url: /go/encryptiontype/
---

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
