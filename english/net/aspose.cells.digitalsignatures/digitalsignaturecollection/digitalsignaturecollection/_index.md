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
// Called: certSigns = new DigitalSignatureCollection();
[TestFixtureSetUp]
#endif
        public void DigitalSignatureCollection_Constructor()
        {
            Aspose.Cells.License license = new Aspose.Cells.License();
            license.SetLicense(Constants.licPath);

            string pfx = dir + "ForTest.pfx";
            string password = "123456";
            string comment = "test";

            certSigns = new DigitalSignatureCollection();
            X509Certificate2 cert = new X509Certificate2(pfx, password);
            Aspose.Cells.DigitalSignatures.DigitalSignature certSign =
                new Aspose.Cells.DigitalSignatures.DigitalSignature(cert, comment, DateTime.Now);
            certSigns.Add(certSign);
        }
```

### See Also

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


