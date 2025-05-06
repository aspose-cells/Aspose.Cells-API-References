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
[Test]
        public void Property_Id()
        {
            string path = Constants.sourcePath + &quot;CELLSNET-47892/&quot;;
            Workbook wb = new Workbook(path + &quot;before_sign.xlsx&quot;);
            SignatureLine signatureLine = wb.Worksheets[0].Pictures[0].SignatureLine;

            X509Certificate2 certificate = new X509Certificate2(path + &quot;rsa2048.pfx&quot;, &quot;123456&quot;);
            Aspose.Cells.DigitalSignatures.DigitalSignature signature =
                new Aspose.Cells.DigitalSignatures.DigitalSignature(certificate, &quot;test Microsoft Office signature line&quot;, DateTime.UtcNow);
            signature.Id = signatureLine.Id;
            signature.ProviderId = signatureLine.ProviderId;
            //sinature text, e.g. your name
            //signature.Text = &quot;signed by Aspose.Cells&quot;;
            //Or signature Image
            signature.Image = File.ReadAllBytes(path + &quot;signer.emf&quot;);

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


