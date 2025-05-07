---
title: Range.RowCount
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the count of rows in the range
type: docs
url: /net/aspose.cells/range/rowcount/
---
## Range.RowCount property

Gets the count of rows in the range.

```csharp
public int RowCount { get; }
```

### Examples

```csharp
// Called: testAreEqual(maxRow, range.RowCount, caseName);
private void Property_RowCount(Workbook workbook,int maxRow)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
            testAreEqual(0, range.FirstRow, caseName);
            testAreEqual(maxRow, range.RowCount, caseName);
            testAreEqual(255, range.FirstColumn, caseName);
            testAreEqual(1, range.ColumnCount, caseName);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


