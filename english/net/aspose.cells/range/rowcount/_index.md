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
// Called: testAreEqual(256, range.RowCount, caseName);
private void Range_Property_RowCount(Workbook workbook,int maxColumn)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
            testAreEqual(0, range.FirstRow, caseName);
            testAreEqual(256, range.RowCount, caseName);
            testAreEqual(0, range.FirstColumn, caseName);
            testAreEqual(maxColumn, range.ColumnCount, caseName);          
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


