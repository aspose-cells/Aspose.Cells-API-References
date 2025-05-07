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
// Called: Assert.IsTrue(wb2.VbaProject.IsSigned);
[Test]
        public void Property_IsSigned()
        {
            Workbook wb = new Workbook(vbaDir + "CELLSNET-43920.xls");
            Assert.IsTrue(wb.VbaProject.IsSigned);
            Assert.IsTrue(wb.VbaProject.IsValidSigned);

            Workbook wb2 = new Workbook(vbaDir + "CELLSNET-43920.xlsb");
            Assert.IsTrue(wb2.VbaProject.IsSigned);
            Assert.IsTrue(wb2.VbaProject.IsValidSigned);
        }
```

### See Also

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


