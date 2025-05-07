---
title: Workbook.SetDigitalSignature
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Sets digital signature to an spreadsheet file Excel2007 and later
type: docs
url: /net/aspose.cells/workbook/setdigitalsignature/
---
## Workbook.SetDigitalSignature method

Sets digital signature to an spreadsheet file (Excel2007 and later).

```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Remarks

Only support adding Xmldsig Digital Signature

### Examples

```csharp
// Called: workbook.SetDigitalSignature(dsCollection);
[Test]
        public void Method_DigitalSignatureCollection_() //relate to CELLSNET-46246
        {
            string password = "1234567890";

            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "CELLSNET-45479/test.xlsx");

            Aspose.Cells.DigitalSignatures.DigitalSignatureCollection dsCollection =
                new Aspose.Cells.DigitalSignatures.DigitalSignatureCollection();

            Aspose.Cells.DigitalSignatures.DigitalSignature signature =
                new Aspose.Cells.DigitalSignatures.DigitalSignature(File.ReadAllBytes(Constants.sourcePath + "CELLSNET-45479/test_dsa_sha1_1024.pfx"), password, 
                "test for sign", DateTime.Now);

            dsCollection.Add(signature);

            workbook.SetDigitalSignature(dsCollection);

            workbook.Save(Constants.destPath + "CELLSNET-45479_BouncyCastle_Cs.xlsx");
            workbook.Dispose();

            Workbook workbook1 = new Workbook(Constants.destPath + "CELLSNET-45479_BouncyCastle_Cs.xlsx");
            foreach (Aspose.Cells.DigitalSignatures.DigitalSignature digitalSignature in workbook1.GetDigitalSignature())
            {
                Assert.IsTrue(digitalSignature.IsValid);
            }

        }
```

### See Also

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


