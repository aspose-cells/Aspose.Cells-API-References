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
// Called: filter.AddFilter(0, "a");
public void AutoFilter_Method_AddFilter()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var filter = workbook.Worksheets[0].ListObjects[0].AutoFilter;
    filter.AddFilter(0, "a");
    filter.AddFilter(0, "e");
    filter.Refresh(true);
    Assert.IsFalse(workbook.Worksheets[0].Cells.Rows[6].IsHidden);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);//.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


