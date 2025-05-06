---
title: Cells.IsRowHidden
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Checks whether a row at given index is hidden
type: docs
url: /net/aspose.cells/cells/isrowhidden/
---
## Cells.IsRowHidden method

Checks whether a row at given index is hidden.

```csharp
public bool IsRowHidden(int rowIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | row index |

### Return Value

true if the row is hidden

### Examples

```csharp
// Called: Assert.IsFalse(cells.IsRowHidden(i), &amp;quot;Row-&amp;quot; + i);
[Test]
        public void Method_Int32_()
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


