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
// Called: dataRange.FirstRow + dataRange.RowCount - 1, dataRange.ColumnCount, ShiftType.Up);
[Test]
        public void Property_FirstRow()
        {
            var size = 1;
            var workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/CellsNet44880.xlsx&quot;);
            var worksheet = workbook.Worksheets[0];
            var list = worksheet.ListObjects[&quot;table1&quot;];
            var dataRange = list.DataRange;
            worksheet.Cells.DeleteRange(dataRange.FirstRow + size, dataRange.FirstColumn,
                dataRange.FirstRow + dataRange.RowCount - 1, dataRange.ColumnCount, ShiftType.Up);

            list.AutoFilter.Sorter.Sort();
            // Got this meesage in result file. 
            // We found a problem with some content in &apos;file&apos;. Do you want us to try to recover as much as we can? If you trust the source of this workbook, click Yes. 
            Util.SaveManCheck(workbook, &quot;Shape&quot;, &quot;CellsNet44880.xlsx&quot;);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


