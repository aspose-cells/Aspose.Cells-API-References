---
title: DigitalSignature.Image
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignature property. Specifies an image for the digital signature. Default value is null
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignature/image/
---
## DigitalSignature.Image property

Specifies an image for the digital signature. Default value is null.

```csharp
public byte[] Image { get; set; }
```

### Examples

```csharp
// Called: signature.Image = File.ReadAllBytes(path + "signer.emf");
[Test]
        public void Property_Image()
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


