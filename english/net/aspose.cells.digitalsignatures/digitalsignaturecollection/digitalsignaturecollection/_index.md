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
// Called: DigitalSignatureCollection BCCertSigns = new DigitalSignatureCollection();
[Test]
        public void DigitalSignatureCollection_Constructor()
        {

            string pfx = dir + &quot;ForTest.pfx&quot;;
            string password = &quot;123456&quot;;
            string comment = &quot;test&quot;;

            DigitalSignatureCollection BCCertSigns = new DigitalSignatureCollection();
            Aspose.Cells.DigitalSignatures.DigitalSignature BCCertSign =
                new Aspose.Cells.DigitalSignatures.DigitalSignature(File.ReadAllBytes(pfx), password, comment, DateTime.Now);
            BCCertSign.XAdESType = XAdESType.XAdES;
            BCCertSigns.Add(BCCertSign);

            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-46998.xlsx&quot;);
            wb.SetDigitalSignature(BCCertSigns);

            wb.Save(Constants.destPath + &quot;CELLSNET-46998_Cs.xlsx&quot;);
        }
```

### See Also

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


