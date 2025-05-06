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
// Called: testAreEqual(3, cell.GetMergedRange().RowCount, caseName);
private void Method_GetMergedRange(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[2, 2];
            testAreEqual(2, cell.GetMergedRange().FirstRow, caseName);
            testAreEqual(2, cell.GetMergedRange().FirstColumn, caseName);
            testAreEqual(3, cell.GetMergedRange().RowCount, caseName);
            testAreEqual(2, cell.GetMergedRange().ColumnCount, caseName);
        }
```

### See Also

* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


