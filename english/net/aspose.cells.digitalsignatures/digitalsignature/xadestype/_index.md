---
title: DigitalSignature.XAdESType
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignature property. XAdES type. Default value is NoneXAdES is off
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignature/xadestype/
---
## DigitalSignature.XAdESType property

XAdES type. Default value is None(XAdES is off).

```csharp
public XAdESType XAdESType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(XAdESType.XAdES, signature.XAdESType);
[Test]
        public void Property_XAdESType()
        {
            string filePath = Constants.sourcePath + &quot;CELLSNET-47117/asposenet_570_src01.xlsx&quot;;
            string certPath = Constants.sourcePath + &quot;CELLSNET-47117/asposenet_570_src02.pfx&quot;;
            string outpPath = Constants.destPath + &quot;CELLSNET-47117_Cs.xlsx&quot;;
            using (Workbook workbook = new Workbook(filePath))
            {
                // get raw data of certificate
                byte[] certificateRawData = File.ReadAllBytes(certPath);
                Aspose.Cells.DigitalSignatures.DigitalSignature signature = new Aspose.Cells.DigitalSignatures.DigitalSignature(certificateRawData, &quot;1234567890&quot;, &quot;comment1&quot;, DateTime.Now);
                signature.XAdESType = Aspose.Cells.DigitalSignatures.XAdESType.XAdES;
                Aspose.Cells.DigitalSignatures.DigitalSignatureCollection collection = new Aspose.Cells.DigitalSignatures.DigitalSignatureCollection();
                collection.Add(signature);
                workbook.SetDigitalSignature(collection);
                workbook.Save(outpPath);
            }
            // try to load file and read signatures from there
            using (Workbook workbook = new Workbook(outpPath))
            {
                Aspose.Cells.DigitalSignatures.DigitalSignatureCollection collection = workbook.GetDigitalSignature();
                foreach (Aspose.Cells.DigitalSignatures.DigitalSignature signature in collection)
                {
                    Assert.AreEqual(XAdESType.XAdES, signature.XAdESType);
                }
            }
        }
```

### See Also

* enum [XAdESType](../../xadestype/)
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


