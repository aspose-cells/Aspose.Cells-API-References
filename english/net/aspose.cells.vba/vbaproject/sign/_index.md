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
// Called: vba.Sign(bcCertSign);
[Test]
        public void Method_DigitalSignature_()
        {
            Workbook wb = new Workbook(vbaDir + &quot;SignXlsm.xlsm&quot;);
            VbaProject vba = wb.VbaProject;
            if (vba != null)
            {
                vba.Sign(bcCertSign);
                string saveFile = Constants.destPath + &quot;VBA_SignXlsm_BC.xlsm&quot;;
                wb.Save(saveFile, SaveFormat.Xlsm);

                Workbook validteWb = new Workbook(saveFile);
                Assert.IsTrue(validteWb.VbaProject.IsSigned);
                Assert.IsTrue(validteWb.VbaProject.IsValidSigned);
            }
        }
```

### See Also

* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


