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
private void Method_GetStyle(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            for (int row = 1; row &lt;= 3; row++)
            {
                checkStyle(cells[row, 2].GetStyle());
            }
            for (int row = 3; row &lt;= 5; row++)
            {
                checkStyle(cells[row, 3].GetStyle());
            }
            checkRowStyle(cells[7, 0].GetStyle());
            checkRowStyle(cells[5, 1].GetStyle());
            checkRowStyle(cells[5, 2].GetStyle());
            for (int col = 3; col &lt;= 8; col++)
            {
                checkRowStyle(cells[7, col].GetStyle());
            }
            checkRowStyle(cells[7, 98].GetStyle());
            checkRowStyle(cells[7, 192].GetStyle());
            checkRowStyle(cells[7, 206].GetStyle());
            checkRowStyle(cells[7, 254].GetStyle());
            checkRowStyle(cells[7, 255].GetStyle());
            checkColumnStyle(cells.Columns[5].GetStyle());
        }
```

### See Also

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


