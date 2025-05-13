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
public void Cell_Property_IsCheckBoxStyle()
{
    Workbook wb = new Workbook();
    Cell cell = wb.Worksheets[0].Cells["B1"];
    cell.IsCheckBoxStyle = true;
    wb.Save(Constants.destPath + "example.xlsx");
    wb = new Workbook(Constants.destPath + "example.xlsx");
    cell = wb.Worksheets[0].Cells["A1"];
    cell.IsCheckBoxStyle = true;
    cell.PutValue(true);
    cell = wb.Worksheets[0].Cells["B1"];
    Assert.IsTrue(cell.IsCheckBoxStyle);
    cell.IsCheckBoxStyle = false;
    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


