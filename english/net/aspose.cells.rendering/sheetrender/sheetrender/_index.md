---
title: SheetRender.SheetRender
second_title: Aspose.Cells for .NET API Reference
description: SheetRender constructor. the construct of SheetRender need worksheet and ImageOrPrintOptions as params
type: docs
url: /net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

the construct of SheetRender, need worksheet and ImageOrPrintOptions as params

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| worksheet | Worksheet | Indicate which spreadsheet to be rendered. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |

### Examples

```csharp
// Called: SheetRender newRender = new SheetRender(sheet, new ImageOrPrintOptions());
public void SheetRender_Constructor()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];
    SheetRender render = new SheetRender(sheet, new ImageOrPrintOptions());
    Assert.AreEqual(1, render.PageCount);

    Cells cells = sheet.Cells;
    PivotField field = pivot.RowFields[0];
    field.IsInsertPageBreaksBetweenItems = true;
    pivot.RefreshData();
    pivot.CalculateData();

    SheetRender newRender = new SheetRender(sheet, new ImageOrPrintOptions());
    Assert.AreEqual(6, newRender.PageCount);

    book.Save(Constants.destPath + "TestIsInsertPageBreaksBetweenItems.xlsx");
}
```

### See Also

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


