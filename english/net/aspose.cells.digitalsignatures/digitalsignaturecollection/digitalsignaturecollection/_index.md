---
title: DigitalSignatureCollection.DigitalSignatureCollection
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignatureCollection constructor. The constructor of DigitalSignatureCollection
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignaturecollection/digitalsignaturecollection/
---
## DigitalSignatureCollection constructor

The constructor of DigitalSignatureCollection.

```csharp
public DigitalSignatureCollection()
```

### Examples

```csharp
// Called: new Aspose.Cells.DigitalSignatures.DigitalSignatureCollection();
[Test]
        public void DigitalSignatureCollection_Constructor()
        {
            string password = "1234567890";

            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "CELLSNET-45479/test.xlsx");

            X509Certificate2 certificate = new X509Certificate2(Constants.sourcePath + "CELLSNET-45479/test_dsa_sha1_1024.pfx", password);

            Aspose.Cells.DigitalSignatures.DigitalSignatureCollection dsCollection =
                new Aspose.Cells.DigitalSignatures.DigitalSignatureCollection();

            Aspose.Cells.DigitalSignatures.DigitalSignature signature =
                new Aspose.Cells.DigitalSignatures.DigitalSignature(certificate, "test for sign", DateTime.Now);

            dsCollection.Add(signature);

            workbook.SetDigitalSignature(dsCollection);

            workbook.Save(Constants.destPath + "CELLSNET-45479_Cs.xlsx");
            workbook.Dispose();

            Workbook workbook1 = new Workbook(Constants.destPath + "CELLSNET-45479_Cs.xlsx");
            foreach (Aspose.Cells.DigitalSignatures.DigitalSignature digitalSignature in workbook1.GetDigitalSignature())
            {
                Assert.IsTrue(digitalSignature.IsValid);
            }

        }
```

### See Also

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


