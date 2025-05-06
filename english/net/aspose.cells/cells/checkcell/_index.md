---
title: Cells.CheckCell
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the Cell element or null at the specified cell row index and column index
type: docs
url: /net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

Gets the [`Cell`](../../cell/) element or null at the specified cell row index and column index.

```csharp
public Cell CheckCell(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
| column | Int32 | Column index |

### Return Value

Return Cell object if a Cell object exists. Return null if the cell does not exist.

### Examples

```csharp
// Called: Assert.AreEqual(cells.CheckCell(0, 10), null);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(&quot;sdfsdf&quot;);
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;
            StyleFlag flag = new StyleFlag();
            flag.All = true;
            cells.Rows[0].ApplyStyle(style, flag);
            cells.ClearContents(0, 0, 1, 0x3FFF);
            Assert.AreEqual(cells.CheckCell(0, 10), null);
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


