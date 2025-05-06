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
        public void Method_DigitalSignatureCollection_()
        {
            string password = &quot;1234567890&quot;;

            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + &quot;CELLSNET-45479/test.xlsx&quot;);

            X509Certificate2 certificate = new X509Certificate2(Constants.sourcePath + &quot;CELLSNET-45479/test_dsa_sha1_1024.pfx&quot;, password);

            Aspose.Cells.DigitalSignatures.DigitalSignatureCollection dsCollection =
                new Aspose.Cells.DigitalSignatures.DigitalSignatureCollection();

            Aspose.Cells.DigitalSignatures.DigitalSignature signature =
                new Aspose.Cells.DigitalSignatures.DigitalSignature(certificate, &quot;test for sign&quot;, DateTime.Now);

            dsCollection.Add(signature);

            workbook.SetDigitalSignature(dsCollection);

            workbook.Save(Constants.destPath + &quot;CELLSNET-45479_Cs.xlsx&quot;);
            workbook.Dispose();

            Workbook workbook1 = new Workbook(Constants.destPath + &quot;CELLSNET-45479_Cs.xlsx&quot;);
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


