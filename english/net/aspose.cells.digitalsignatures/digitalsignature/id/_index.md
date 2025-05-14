---
title: DigitalSignature.Id
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignature property. Specifies a GUID which can be crossreferenced with the GUID of the signature line stored in the document content. Default value is Empty all zeroes Guid
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignature/id/
---
## DigitalSignature.Id property

Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Default value is Empty (all zeroes) Guid.

```csharp
public Guid Id { get; set; }
```

### Remarks

When set, it associates [`SignatureLine`](../../../aspose.cells.drawing/signatureline/) with corresponding [`DigitalSignature`](../).

### Examples

```csharp
// Called: signature.Id = signatureLine.Id;
public void DigitalSignature_Property_Id()
{
    string path = Constants.sourcePath + "CELLSNET-47892/";
    Workbook wb = new Workbook(path + "before_sign.xlsx");
    SignatureLine signatureLine = wb.Worksheets[0].Pictures[0].SignatureLine;

    X509Certificate2 certificate = new X509Certificate2(path + "rsa2048.pfx", "123456");
    Aspose.Cells.DigitalSignatures.DigitalSignature signature =
        new Aspose.Cells.DigitalSignatures.DigitalSignature(certificate, "test Microsoft Office signature line", DateTime.UtcNow);
    signature.Id = signatureLine.Id;
    signature.ProviderId = signatureLine.ProviderId;
    //sinature text, e.g. your name
    //signature.Text = "signed by Aspose.Cells";
    //Or signature Image
    signature.Image = File.ReadAllBytes(path + "signer.emf");

    Aspose.Cells.DigitalSignatures.DigitalSignatureCollection dsCollection = new Aspose.Cells.DigitalSignatures.DigitalSignatureCollection();
    dsCollection.Add(signature);
    wb.SetDigitalSignature(dsCollection);

    MemoryStream ms = new MemoryStream();
    wb.Save(ms, SaveFormat.Xlsx);

    ms.Position = 0;
    Workbook reloadedWb = new Workbook(ms);
    foreach(Aspose.Cells.DigitalSignatures.DigitalSignature validateSignature in reloadedWb.GetDigitalSignature())
    {
        Assert.IsTrue(validateSignature.IsValid);
    }
}
```

### See Also

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


