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
// Called: DigitalSignatureCollection signs = wb2.GetDigitalSignature();
[Test]
        public void Method_GetDigitalSignature()
        {
            MemoryStream ms = new MemoryStream();
            Workbook wb = new Workbook(dir + "XlsxSignValidate.xlsx");
            wb.SetDigitalSignature(certSigns);
            wb.Save(ms, SaveFormat.Xlsx);

            Workbook wb2 = new Workbook(ms);
            DigitalSignatureCollection signs = wb2.GetDigitalSignature();

            foreach (Aspose.Cells.DigitalSignatures.DigitalSignature sign in signs)
            {
                Assert.IsTrue(sign.IsValid);
            }

            ms.Dispose();
        }
```

### See Also

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


