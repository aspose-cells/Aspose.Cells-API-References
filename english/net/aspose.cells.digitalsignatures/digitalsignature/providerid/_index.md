---
title: DigitalSignature.ProviderId
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignature property. Specifies the class ID of the signature provider. Default value is Empty all zeroes Guid
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignature/providerid/
---
## DigitalSignature.ProviderId property

Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid.

```csharp
public Guid ProviderId { get; set; }
```

### Remarks

The cryptographic service provider (CSP) is an independent software module that actually performs cryptography algorithms for authentication, encoding, and encryption. Microsoft Office reserves the value of {00000000-0000-0000-0000-000000000000} for its default signature provider, and {000CD6A4-0000-0000-C000-000000000046} for its East Asian signature provider. The GUID of the additionally installed provider should be obtained from the documentation shipped with the provider.

### Examples

```csharp
// Called: signature.ProviderId = signatureLine.ProviderId;
[Test]
        public void Property_ProviderId()
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


