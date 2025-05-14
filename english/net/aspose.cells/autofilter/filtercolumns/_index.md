---
title: AutoFilter.FilterColumns
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter property. Gets the collection of the filter columns
type: docs
url: /net/aspose.cells/autofilter/filtercolumns/
---
## AutoFilter.FilterColumns property

Gets the collection of the filter columns.

```csharp
public FilterColumnCollection FilterColumns { get; }
```

### Examples

```csharp
// Called: FilterColumn fc = autoFilter.FilterColumns[2];
public void AutoFilter_Property_FilterColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    AutoFilter autoFilter = workbook.Worksheets[0].AutoFilter;
    int maxColRange = workbook.Worksheets[0].Cells.MaxDataColumn;
    autoFilter.Range = ("A1:" + CellsHelper.ColumnIndexToName(maxColRange) + "1");

    autoFilter.Filter(2, "present");
    FilterColumn fc = autoFilter.FilterColumns[2];
    //  autoFilter.FilterColumns[0].Filter;
    autoFilter.Refresh();
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);//.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


