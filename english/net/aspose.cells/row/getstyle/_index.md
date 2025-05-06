---
title: Row.GetStyle
second_title: Aspose.Cells for .NET API Reference
description: Row method. Gets the style of this row
type: docs
url: /net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

Gets the style of this row.

```csharp
public Style GetStyle()
```

### Remarks

Modifying the returned style object directly takes no effect for this row or any cells in this row. You have to call [`ApplyStyle`](../applystyle/) or [`SetStyle`](../setstyle/) method to apply the change to this row. Row's style is the style which will be inherited by cells in this row(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)

### Examples

```csharp
// Called: checkRowStyle(cells.Rows[7].GetStyle());
private void Method_GetStyle(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            checkStyle(cells[3, 4].GetStyle());
            checkStyle(cells[3, 5].GetStyle());
            checkStyle(cells[4, 2].GetStyle());
            checkStyle(cells[4, 3].GetStyle());
            checkStyle(cells[5, 2].GetStyle());
            checkStyle(cells[5, 3].GetStyle());

            checkRowStyle(cells.Rows[7].GetStyle());
            checkColumnStyle(cells[0, 5].GetStyle());
            checkColumnStyle(cells[1, 5].GetStyle());
            checkColumnStyle(cells[2, 7].GetStyle());
            testAreEqual(false, cells[2, 5].IsStyleSet, caseName);
            checkColumnStyle(cells[3, 7].GetStyle());
            for (int row = 4; row &lt;= 6; row++)
            {
                checkColumnStyle(cells[row, 5].GetStyle());
            }
            checkColumnStyle(cells[99, 5].GetStyle());
            checkColumnStyle(cells[256, 5].GetStyle());
            checkColumnStyle(cells[1671, 5].GetStyle());
            checkColumnStyle(cells[25610, 5].GetStyle());
            checkColumnStyle(cells[65534, 5].GetStyle());
            checkColumnStyle(cells[65535, 5].GetStyle());
        }
```

### See Also

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


