---
title: Column.GetStyle
second_title: Aspose.Cells for .NET API Reference
description: Column method. Gets the style of this column
type: docs
url: /net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

Gets the style of this column.

```csharp
public Style GetStyle()
```

### Remarks

Modifying the returned style object directly takes no effect for this column or any cells in this column. You have to call [`ApplyStyle`](../applystyle/) or [`SetStyle`](../setstyle/) method to apply the change to this column. Column's style is the style which will be inherited by cells in this column(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)

### Examples

```csharp
// Called: checkColumnStyle(cells.Columns[5].GetStyle());
private void Column_Method_GetStyle(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            checkRangeStyle(cells);
            testAreEqual(false, cells[7, 0].IsStyleSet, caseName);
            testAreEqual(false, cells[7, 1].IsStyleSet, caseName);
            checkRowStyle(cells[7, 2].GetStyle());
            checkRowStyle(cells[7, 30].GetStyle());
            checkRowStyle(cells[7, 76].GetStyle());
            checkRowStyle(cells[7, 129].GetStyle());
            checkRowStyle(cells[7, 255].GetStyle());
            checkColumnStyle(cells.Columns[5].GetStyle());
        }
```

### See Also

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


