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
// Called: signature.Image = File.ReadAllBytes(path + &amp;quot;signer.emf&amp;quot;);
[Test]
        public void Property_Image()
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


