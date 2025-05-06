---
title: WorksheetCollection.GetNamedRangesAndTables
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Gets all predefined named ranges in the spreadsheet
type: docs
url: /net/aspose.cells/worksheetcollection/getnamedrangesandtables/
---
## WorksheetCollection.GetNamedRangesAndTables method

Gets all pre-defined named ranges in the spreadsheet.

```csharp
public Range[] GetNamedRangesAndTables()
```

### Return Value

An array of Range objects.

Returns null if the named range does not exist.

### Examples

```csharp
// Called: Aspose.Cells.Range[] rs = workbook.Worksheets.GetNamedRangesAndTables();
[Test]
        public void Method_GetNamedRangesAndTables()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet27760.xlsx&quot;);
            Aspose.Cells.Range[] rs = workbook.Worksheets.GetNamedRangesAndTables();
            Assert.AreEqual(rs.Length, 4);
        }
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


