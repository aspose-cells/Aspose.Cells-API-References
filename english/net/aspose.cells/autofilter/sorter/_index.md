---
title: AutoFilter.Sorter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter property. Gets the data sorter
type: docs
url: /net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

Gets the data sorter.

```csharp
public DataSorter Sorter { get; }
```

### Examples

```csharp
// Called: list.AutoFilter.Sorter.Sort();
public void AutoFilter_Property_Sorter()
{
    var size = 1;
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var worksheet = workbook.Worksheets[0];
    var list = worksheet.ListObjects["table1"];
    var dataRange = list.DataRange;
    worksheet.Cells.DeleteRange(dataRange.FirstRow + size, dataRange.FirstColumn,
        dataRange.FirstRow + dataRange.RowCount - 1, dataRange.ColumnCount, ShiftType.Up);

    list.AutoFilter.Sorter.Sort();
    // Got this meesage in result file. 
    // We found a problem with some content in 'file'. Do you want us to try to recover as much as we can? If you trust the source of this workbook, click Yes. 
    Util.SaveManCheck(workbook, "Shape", "example.xlsx");
}
```

### See Also

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


