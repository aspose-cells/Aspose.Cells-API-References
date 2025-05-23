---
title: Style.Borders
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets the BorderCollection of the style
type: docs
url: /net/aspose.cells/style/borders/
---
## Style.Borders property

Gets the [`BorderCollection`](../../bordercollection/) of the style.

```csharp
public BorderCollection Borders { get; }
```

### Examples

```csharp
// Called: style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
public void Style_Property_Borders()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Style style = cells[1, 1].GetStyle();
    style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
    cells[1, 1].SetStyle(style);

    checkCellBorderType_Medium(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkCellBorderType_Medium(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkCellBorderType_Medium(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
    checkCellBorderType_Medium(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


