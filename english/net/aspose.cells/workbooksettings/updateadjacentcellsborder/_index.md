---
title: WorkbookSettings.UpdateAdjacentCellsBorder
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether update adjacent cells border
type: docs
url: /net/aspose.cells/workbooksettings/updateadjacentcellsborder/
---
## WorkbookSettings.UpdateAdjacentCellsBorder property

Indicates whether update adjacent cells' border.

```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```

### Remarks

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

### Examples

```csharp
// Called: workbook.Settings.UpdateAdjacentCellsBorder = true;
public void WorkbookSettings_Property_UpdateAdjacentCellsBorder()
{
    var workbook = new Workbook();
    workbook.Settings.UpdateAdjacentCellsBorder = true;
    var worksheet = workbook.Worksheets[0];
    worksheet.Cells[0, 0].Value = "hello";
    //create range and style and apply horizontal style to A1 cell
    var range = worksheet.Cells.CreateRange(0, 0, 1, 1);
    var style = worksheet.Workbook.CreateStyle();
    var flag = new StyleFlag();
    style.HorizontalAlignment = TextAlignmentType.Center;
    flag.HorizontalAlignment = true;
    range.ApplyStyle(style, flag);

    //create another range and style and apply vertical alignment to A1 cell
    range = worksheet.Cells.CreateRange(0, 0, 1, 1);
    style = worksheet.Workbook.CreateStyle();
    flag = new StyleFlag();
    style.VerticalAlignment = TextAlignmentType.Center;
    flag.VerticalAlignment = true;
    range.ApplyStyle(style, flag);

    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(TextAlignmentType.Center, workbook.Worksheets[0].Cells["A1"].GetStyle().VerticalAlignment);
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


