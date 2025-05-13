---
title: DigitalSignature.IsValid
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignature property. If this digital signature is valid and the document has not been tampered with this value will be true
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignature/isvalid/
---
## DigitalSignature.IsValid property

If this digital signature is valid and the document has not been tampered with, this value will be true.

```csharp
public bool IsValid { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(sign.IsValid);
public void DigitalSignature_Property_IsValid()
{
    Workbook wb = new Workbook(dir + "example.xlsx");

    DigitalSignatureCollection signs = wb.GetDigitalSignature();

    foreach (Aspose.Cells.DigitalSignatures.DigitalSignature sign in signs)
    {
        Assert.IsTrue(sign.IsValid);
    }
}
```

### See Also

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


