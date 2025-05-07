---
title: Range.FirstRow
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the index of the first row of the range
type: docs
url: /net/aspose.cells/range/firstrow/
---
## Range.FirstRow property

Gets the index of the first row of the range.

```csharp
public int FirstRow { get; }
```

### Examples

```csharp
// Called: testAreEqual(0, range.FirstRow, caseName);
private void Property_FirstRow(Workbook workbook,int maxColumn)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");        
            testAreEqual(0, range.FirstRow, caseName);
            testAreEqual(2, range.RowCount, caseName);
            testAreEqual(0, range.FirstColumn, caseName);
            testAreEqual(maxColumn, range.ColumnCount, caseName);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


