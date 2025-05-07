---
title: RowCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: RowCollection property. Gets a Row object by given row index. The Row object of given row index will be instantiated if it does not exist before
type: docs
url: /net/aspose.cells/rowcollection/item/
---
## RowCollection indexer

Gets a [`Row`](../../row/) object by given row index. The Row object of given row index will be instantiated if it does not exist before.

```csharp
public Row this[int rowIndex] { get; }
```

### Examples

```csharp
// Called: Style style = cells.Rows[7].GetStyle();
private void Property_Int32_(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            for (int row = 3; row <= 5; row++)
            {
                for (int col = 2; col <= 3; col++)
                {
                    CheckStyle(cells[row, col].GetStyle());
                }
            }
            Style style = cells.Rows[7].GetStyle();
            AssertHelper.equals(Color.Blue, style.ForegroundColor, "cells.Rows[7].Style.ForegroundColor");
            AssertHelper.AreEqual(BackgroundType.Solid, style.Pattern, "cells.Rows[7].Style.Pattern");
            style = cells.Columns[5].GetStyle();
            AssertHelper.equals(Color.Red, style.ForegroundColor, "cells.Columns[5].Style.ForegroundColor");
            AssertHelper.AreEqual(BackgroundType.Solid, style.Pattern, "cells.Columns[5].Style.Pattern");
        }
```

### See Also

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


