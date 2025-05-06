---
title: VbaProject.IsSigned
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Indicates whether VBAcode is signed or not
type: docs
url: /net/aspose.cells.vba/vbaproject/issigned/
---
## VbaProject.IsSigned property

Indicates whether VBAcode is signed or not.

```csharp
public bool IsSigned { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(wb.VbaProject.IsSigned);
[Test]
        public void Property_IsSigned()
        {
            Workbook wb = new Workbook(vbaDir + &quot;ValidateXlsm.xlsm&quot;);
            Assert.IsTrue(wb.VbaProject.IsSigned);
            Assert.IsTrue(wb.VbaProject.IsValidSigned);

            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);

            Workbook validateWb = new Workbook(ms);
            Assert.IsTrue(validateWb.VbaProject.IsSigned);
            Assert.IsTrue(validateWb.VbaProject.IsValidSigned);

            ms.Dispose();
        }
```

### See Also

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


