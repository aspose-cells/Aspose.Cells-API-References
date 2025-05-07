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
// Called: signature.XAdESType = Aspose.Cells.DigitalSignatures.XAdESType.XAdES;
[Test]
        public void Property_XAdESType()
        {
            string filePath = Constants.sourcePath + "CELLSNET-47117/asposenet_570_src01.xlsx";
            string certPath = Constants.sourcePath + "CELLSNET-47117/asposenet_570_src02.pfx";
            string outpPath = Constants.destPath + "CELLSNET-47117_Cs.xlsx";
            using (Workbook workbook = new Workbook(filePath))
            {
                // get raw data of certificate
                byte[] certificateRawData = File.ReadAllBytes(certPath);
                Aspose.Cells.DigitalSignatures.DigitalSignature signature = new Aspose.Cells.DigitalSignatures.DigitalSignature(certificateRawData, "1234567890", "comment1", DateTime.Now);
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


