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
// Called: style = cells.Columns[5].GetStyle();
private void Method_GetStyle(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            for (int row = 3; row <= 5; row++)
            {
                for (int col = 2; col <= 3; col++)
                {
                    CheckStyle(cells[row, col].GetStyle());
                }
            }
            AssertHelper.AreEqual(BackgroundType.HorizontalStripe, cells[6, 2].GetStyle().Pattern, "cells[6, 2].GetStyle().Pattern");
            AssertHelper.equals(Color.Green, cells[6, 2].GetStyle().ForegroundColor, "cells[6, 2].GetStyle().BackgroundColor");
            AssertHelper.AreEqual(BackgroundType.HorizontalStripe, cells[6, 3].GetStyle().Pattern, "cells[6, 3].GetStyle().Pattern");
            AssertHelper.equals(Color.Green, cells[6, 3].GetStyle().ForegroundColor, "cells[6, 3].GetStyle().BackgroundColor");
            Style style = cells.Rows[8].GetStyle();
            AssertHelper.equals(Color.Blue, style.ForegroundColor, "cells.Rows[8].Style.ForegroundColor");
            AssertHelper.AreEqual(BackgroundType.Solid, style.Pattern, "cells.Rows[8].Style.Pattern");
            style = cells.Columns[5].GetStyle();
            AssertHelper.equals(Color.Red, style.ForegroundColor, "cells.Columns[5].Style.ForegroundColor");
            AssertHelper.AreEqual(BackgroundType.Solid, style.Pattern, "cells.Columns[5].Style.Pattern");
        }
```

### See Also

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


