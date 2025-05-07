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
            Workbook workbook = new Workbook(Constants.HtmlSourcePath + "AutoFilter_001_h.xls");
            workbook.Save(Constants.HtmlDestPath + "AutoFilter_001_h.html");
            workbook = new Workbook(Constants.HtmlDestPath + "AutoFilter_001_h.html");
            AutoFilter autoFilter = workbook.Worksheets[0].AutoFilter;
            FilterColumn fc = autoFilter.FilterColumns[2];
            CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
            Assert.AreEqual(fc.FilterType, FilterType.CustomFilters);
            Console.WriteLine(cf.Criteria.ToString(), "7");
        }
```

### See Also

* class [CustomFilter](../../customfilter/)
* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


