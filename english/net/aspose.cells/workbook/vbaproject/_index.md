---
title: Workbook.VbaProject
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the VbaProject in a spreadsheet
type: docs
url: /net/aspose.cells/workbook/vbaproject/
---
## Workbook.VbaProject property

Gets the `VbaProject` in a spreadsheet.

```csharp
public VbaProject VbaProject { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(validateWb.VbaProject.IsValidSigned);
[Test]
        public void Property_VbaProject()
        {
            Workbook wb = new Workbook(vbaDir + "CELLSNET-43878.xlsm");
            Assert.IsTrue(wb.VbaProject.IsSigned);
            Assert.IsTrue(wb.VbaProject.IsValidSigned);

            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);

            Workbook validateWb = new Workbook(ms);
            Assert.IsTrue(validateWb.VbaProject.IsSigned);
            Assert.IsTrue(validateWb.VbaProject.IsValidSigned);
        }
```

### See Also

* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


