---
title: DigitalSignatureCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignatureCollection method. Add one signature to DigitalSignatureCollection
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/
---
## DigitalSignatureCollection.Add method

Add one signature to DigitalSignatureCollection.

```csharp
public void Add(DigitalSignature digitalSignature)
```

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | DigitalSignature | Digital signature in collection. |

### Examples

```csharp
// Called: dsCollection.Add(signature);
public void DigitalSignatureCollection_Method_Add()
{
    string password = "1234567890";

    Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xlsx");

    X509Certificate2 certificate = new X509Certificate2(Constants.sourcePath + "CELLSNET-45479/test_dsa_sha1_1024.pfx", password);

    Aspose.Cells.DigitalSignatures.DigitalSignatureCollection dsCollection =
        new Aspose.Cells.DigitalSignatures.DigitalSignatureCollection();

    Aspose.Cells.DigitalSignatures.DigitalSignature signature =
        new Aspose.Cells.DigitalSignatures.DigitalSignature(certificate, "test for sign", DateTime.Now);

    dsCollection.Add(signature);

    workbook.SetDigitalSignature(dsCollection);

    workbook.Save(Constants.destPath + "example.xlsx");
    workbook.Dispose();

    Workbook workbook1 = new Workbook(Constants.destPath + "example.xlsx");
    foreach (Aspose.Cells.DigitalSignatures.DigitalSignature digitalSignature in workbook1.GetDigitalSignature())
    {
        Assert.IsTrue(digitalSignature.IsValid);
    }

}
```

### See Also

* class [DigitalSignature](../../digitalsignature/)
* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


