---
title: Enum FilterType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FilterType enum. The filter type
type: docs
url: /net/aspose.cells/filtertype/
---
## FilterType enumeration

The filter type.

```csharp
public enum FilterType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| ColorFilter | `0` | Filter by fill color of the cell. |
| CustomFilters | `1` | Custom filter type. |
| DynamicFilter | `2` | Dynamic filter type. |
| MultipleFilters | `3` | When multiple values are chosen to filter by, or when a group of date values are chosen to filter by, this element groups those criteria together. |
| IconFilter | `4` | Filter by icon of conditional formatting. |
| Top10 | `5` | Top 10 filter. |
| None | `6` | No filter. |

### Examples

```csharp
// Called: Assert.AreEqual(fc.FilterType, FilterType.CustomFilters);
[Test]
        public void Type_FilterType()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


