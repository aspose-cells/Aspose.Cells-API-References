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
// Called: Console.WriteLine(cf.Criteria.ToString(), &amp;quot;7&amp;quot;);
[Test]
        public void Property_Criteria()
        {
            Workbook workbook = new Workbook(Constants.HtmlSourcePath + &quot;AutoFilter_001_h.xls&quot;);
            workbook.Save(Constants.HtmlDestPath + &quot;AutoFilter_001_h.html&quot;);
            workbook = new Workbook(Constants.HtmlDestPath + &quot;AutoFilter_001_h.html&quot;);
            AutoFilter autoFilter = workbook.Worksheets[0].AutoFilter;
            FilterColumn fc = autoFilter.FilterColumns[2];
            CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
            Assert.AreEqual(fc.FilterType, FilterType.CustomFilters);
            Console.WriteLine(cf.Criteria.ToString(), &quot;7&quot;);
        }
```

### See Also

* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


