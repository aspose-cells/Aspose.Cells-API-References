---
title: FilterColumnCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: FilterColumnCollection property. Gets FilterColumn object at the special field
type: docs
url: /net/aspose.cells/filtercolumncollection/item/
---
## FilterColumnCollection indexer

Gets [`FilterColumn`](../../filtercolumn/) object at the special field.

```csharp
public FilterColumn this[int fieldIndex] { get; }
```

| Parameter | Description |
| --- | --- |
| fieldIndex | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### Return Value

Returns [`FilterColumn`](../../filtercolumn/) object.

### Examples

```csharp
// Called: FilterColumn fc = autoFilter.FilterColumns[2];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/CELLSJAVA42502.xlsx&quot;);

            AutoFilter autoFilter = workbook.Worksheets[0].AutoFilter;
            int maxColRange = workbook.Worksheets[0].Cells.MaxDataColumn;
            autoFilter.Range = (&quot;A1:&quot; + CellsHelper.ColumnIndexToName(maxColRange) + &quot;1&quot;);

            autoFilter.Filter(2, &quot;present&quot;);
            FilterColumn fc = autoFilter.FilterColumns[2];
            //  autoFilter.FilterColumns[0].Filter;
            autoFilter.Refresh();
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);//.Save(Constants.destPath + &quot;CELLSJAVA42502.xlsx&quot;);
        }
```

### See Also

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


