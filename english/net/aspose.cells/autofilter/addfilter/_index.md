---
title: AutoFilter.AddFilter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Adds a filter for a filter column
type: docs
url: /net/aspose.cells/autofilter/addfilter/
---
## AutoFilter.AddFilter method

Adds a filter for a filter column.

```csharp
public void AddFilter(int fieldIndex, string criteria)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |

### Remarks

MS Excel 2007 supports multiple selection in a filter column.

### Examples

```csharp
// Called: autoFilter.AddFilter(0, null);
[Test]
        public void Method_String_()
        {
            var wb = new Workbook(Constants.sourcePath + "CellsNet55063.xlsx");
            var ws = wb.Worksheets["Sheet1"];
            var autoFilter = ws.AutoFilter;

        

            autoFilter.AddFilter(0, null);
            autoFilter.AddFilter(0, "");
            autoFilter.Refresh();
            Assert.AreEqual(FilterType.MultipleFilters, autoFilter.FilterColumns[0].FilterType);
            MultipleFilterCollection multiFilters = (MultipleFilterCollection)autoFilter.FilterColumns[0].Filter;
            Assert.IsTrue(multiFilters.MatchBlank);
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


