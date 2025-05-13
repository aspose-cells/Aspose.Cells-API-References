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
// Called: c = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
public void FilterColumnCollection_Property_Item()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    AutoFilter filter = wb.Worksheets[0].AutoFilter;
    CustomFilter c = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
    Assert.AreEqual(FilterOperatorType.Contains, c.FilterOperatorType);
    Assert.AreEqual("e", (string)c.Criteria);
    c.FilterOperatorType = FilterOperatorType.EndsWith;
    Assert.AreEqual("e", (string)c.Criteria);
    Util.ReSave(wb, SaveFormat.Xlsx);//.Save(Constants.destPath + "example.xlsx");

    wb = new Workbook(Constants.sourcePath + "example.xlsx");
    filter = wb.Worksheets[0].AutoFilter;
    filter.Custom(0, FilterOperatorType.NotContains, "e");
    //wb.Save(Constants.destPath + "example.xlsx");
    wb = Util.ReSave(wb, SaveFormat.Xlsx);// new Workbook(Constants.destPath + "example.xlsx");
    filter = wb.Worksheets[0].AutoFilter;
    c = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
    Assert.AreEqual(FilterOperatorType.NotContains, c.FilterOperatorType);
    Assert.AreEqual("e", (string)c.Criteria);
}
```

### See Also

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


