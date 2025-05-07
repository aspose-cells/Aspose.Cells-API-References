---
title: Cell.IsCheckBoxStyle
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether setting this cell as a check box
type: docs
url: /net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

Indicates whether setting this cell as a check box.

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### Examples

```csharp
// Called: cell.IsCheckBoxStyle = false;
[Test]
        public void Property_IsCheckBoxStyle()
        {
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells["B1"];
            cell.IsCheckBoxStyle = true;
            wb.Save(Constants.destPath + "CELLSNET56466.xlsx");
            wb = new Workbook(Constants.destPath + "CELLSNET56466.xlsx");
            cell = wb.Worksheets[0].Cells["A1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(true);
            cell = wb.Worksheets[0].Cells["B1"];
            Assert.IsTrue(cell.IsCheckBoxStyle);
            cell.IsCheckBoxStyle = false;
            wb.Save(Constants.destPath + "CELLSNET564661.xlsx");
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


