---
title: DigitalSignature.ProviderId
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignature property. Specifies the class ID of the signature provider. Default value is Empty all zeroes Guid
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignature/providerid/
---
## DigitalSignature.ProviderId property

Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid.

```csharp
public Guid ProviderId { get; set; }
```

### Remarks

The cryptographic service provider (CSP) is an independent software module that actually performs cryptography algorithms for authentication, encoding, and encryption. Microsoft Office reserves the value of {00000000-0000-0000-0000-000000000000} for its default signature provider, and {000CD6A4-0000-0000-C000-000000000046} for its East Asian signature provider. The GUID of the additionally installed provider should be obtained from the documentation shipped with the provider.

### See Also

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


