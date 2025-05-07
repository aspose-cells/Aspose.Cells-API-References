---
title: Cells.Columns
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the collection of Column objects that represents the individual columns in this worksheet
type: docs
url: /net/aspose.cells/cells/columns/
---
## Cells.Columns property

Gets the collection of [`Column`](../../column/) objects that represents the individual columns in this worksheet.

```csharp
public ColumnCollection Columns { get; }
```

### Examples

```csharp
// Called: style = cells.Columns[6].GetStyle();
private void Property_Columns(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            for (int row = 3; row <= 5; row++)
            {
                for (int col = 3; col <= 4; col++)
                {
                    CheckStyle(cells[row, col].GetStyle());
                }
            }
            Style style = cells.Rows[7].GetStyle();
            AssertHelper.equals(Color.Blue, style.ForegroundColor, "cells.Rows[7].Style.ForegroundColor");
            AssertHelper.AreEqual(BackgroundType.Solid, style.Pattern, "cells.Rows[7].Style.Pattern");
            style = cells.Columns[6].GetStyle();
            AssertHelper.equals(Color.Red, style.ForegroundColor, "cells.Columns[6].Style.ForegroundColor");
            AssertHelper.AreEqual(BackgroundType.Solid, style.Pattern, "cells.Columns[6].Style.Pattern");
        }
```

### See Also

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


