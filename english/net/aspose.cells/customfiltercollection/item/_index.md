---
title: CustomFilterCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: CustomFilterCollection property. Gets the custom filter in the specific index
type: docs
url: /net/aspose.cells/customfiltercollection/item/
---
## CustomFilterCollection indexer

Gets the custom filter in the specific index.

```csharp
public CustomFilter this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
[Test]
        public void Property_Int32_()
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

* class [CustomFilter](../../customfilter/)
* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


