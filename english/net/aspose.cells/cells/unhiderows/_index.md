---
title: Cells.UnhideRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Unhides the hidden rows
type: docs
url: /net/aspose.cells/cells/unhiderows/
---
## Cells.UnhideRows method

Unhides the hidden rows.

```csharp
public void UnhideRows(int row, int totalRows, double height)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| totalRows | Int32 | The row number. |
| height | Double | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |

### Examples

```csharp
// Called: cells.UnhideRows(0, 4, -1);
[Test]
        public void Method_Double_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells.IsDefaultRowHidden = true;
            cells[0, 0].PutValue(1);
            cells[3, 0].PutValue(4);
            cells.UnhideRows(0, 4, -1);
            for (int i = 0; i &lt; 4; i++)
            {
                Assert.IsFalse(cells.IsRowHidden(i), &quot;Row-&quot; + i);
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


