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
// Called: BCCertSign.XAdESType = XAdESType.XAdES;
public void DigitalSignature_Property_XAdESType()
{

    string pfx = dir + "ForTest.pfx";
    string password = "123456";
    string comment = "test";

    DigitalSignatureCollection BCCertSigns = new DigitalSignatureCollection();
    Aspose.Cells.DigitalSignatures.DigitalSignature BCCertSign =
        new Aspose.Cells.DigitalSignatures.DigitalSignature(File.ReadAllBytes(pfx), password, comment, DateTime.Now);
    BCCertSign.XAdESType = XAdESType.XAdES;
    BCCertSigns.Add(BCCertSign);

    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    wb.SetDigitalSignature(BCCertSigns);

    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [XAdESType](../../xadestype/)
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


