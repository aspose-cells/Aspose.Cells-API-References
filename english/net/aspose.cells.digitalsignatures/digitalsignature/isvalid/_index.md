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
[Test]
        public void Property_IsValid()
        {
            MemoryStream ms = new MemoryStream();
            Workbook wb = new Workbook(dir + &quot;XlsSignValidate.xls&quot;);
            wb.SetDigitalSignature(certSigns);
            wb.Save(ms, SaveFormat.Excel97To2003);

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

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


