---
title: Workbook.GetDigitalSignature
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Gets digital signature from file
type: docs
url: /net/aspose.cells/workbook/getdigitalsignature/
---
## Workbook.GetDigitalSignature method

Gets digital signature from file.

```csharp
public DigitalSignatureCollection GetDigitalSignature()
```

### Examples

```csharp
// Called: DigitalSignatureCollection signs = wb.GetDigitalSignature();
public void Workbook_Method_GetDigitalSignature()
{
    Workbook wb = new Workbook(dir + "example.xls");

    DigitalSignatureCollection signs = wb.GetDigitalSignature();

    foreach (Aspose.Cells.DigitalSignatures.DigitalSignature sign in signs)
    {
        Assert.IsTrue(sign.IsValid);
    }
}
```

### See Also

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


