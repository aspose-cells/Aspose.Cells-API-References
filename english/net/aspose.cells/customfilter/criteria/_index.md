---
title: CustomFilter.Criteria
second_title: Aspose.Cells for .NET API Reference
description: CustomFilter property. Gets and sets the criteria
type: docs
url: /net/aspose.cells/customfilter/criteria/
---
## CustomFilter.Criteria property

Gets and sets the criteria.

```csharp
public object Criteria { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(cf.Criteria.ToString(), "7");
public void CustomFilter_Property_Criteria()
{
    Workbook workbook = new Workbook(Constants.HtmlSourcePath + "example.xls");
    workbook.Save(Constants.HtmlDestPath + "example.html");
    workbook = new Workbook(Constants.HtmlDestPath + "example.html");
    AutoFilter autoFilter = workbook.Worksheets[0].AutoFilter;
    FilterColumn fc = autoFilter.FilterColumns[2];
    CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
    Assert.AreEqual(fc.FilterType, FilterType.CustomFilters);
    Console.WriteLine(cf.Criteria.ToString(), "7");
}
```

### See Also

* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


