---
title: VbaProject.Sign
second_title: Aspose.Cells for .NET API Reference
description: VbaProject method. Sign this VBA project by a DigitalSignature
type: docs
url: /net/aspose.cells.vba/vbaproject/sign/
---
## VbaProject.Sign method

Sign this VBA project by a DigitalSignature

```csharp
public void Sign(DigitalSignature digitalSignature)
```

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### Examples

```csharp
// Called: vba.Sign(certSign);
public void VbaProject_Method_Sign()
{
    Workbook wb = new Workbook(vbaDir + "SignXlsm.xlsm");
    VbaProject vba = wb.VbaProject;
    if (vba != null)
    {
        vba.Sign(certSign);
        MemoryStream ms = new MemoryStream();
        wb.Save(ms, SaveFormat.Xlsm);

        Workbook validteWb = new Workbook(ms);
        Assert.IsTrue(validteWb.VbaProject.IsSigned);
        Assert.IsTrue(validteWb.VbaProject.IsValidSigned);

        ms.Dispose();
    }
}
```

### See Also

* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


