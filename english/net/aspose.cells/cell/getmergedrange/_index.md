---
title: Cell.GetMergedRange
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Returns a Range object which represents a merged range
type: docs
url: /net/aspose.cells/cell/getmergedrange/
---
## Cell.GetMergedRange method

Returns a [`Range`](../../range/) object which represents a merged range.

```csharp
public Range GetMergedRange()
```

### Return Value

[`Range`](../../range/) object. Null if this cell is not merged.

### Examples

```csharp
// Called: testAreEqual(cells[1, 1].GetMergedRange().ColumnCount, cells[3, 1].GetMergedRange().ColumnCount, caseName);
private void Method_GetMergedRange(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual(true, cells[3, 1].IsMerged, caseName);
            testAreEqual(cells[1, 1].GetMergedRange().RowCount, cells[3, 1].GetMergedRange().RowCount, caseName);
            testAreEqual(cells[1, 1].GetMergedRange().ColumnCount, cells[3, 1].GetMergedRange().ColumnCount, caseName);
        }
```

### See Also

* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


