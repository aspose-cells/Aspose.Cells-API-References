---
title: AutoFilter.Filter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Filters a list with specified criteria
type: docs
url: /net/aspose.cells/autofilter/filter/
---
## AutoFilter.Filter method

Filters a list with specified criteria.

```csharp
public void Filter(int fieldIndex, string criteria)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). |

### Remarks

Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2003.

### Examples

```csharp
// Called: autofilter1.Filter(0, &amp;quot;A&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;AutoFilter/N22617.xls&quot;);

            Worksheet sheet = wb.Worksheets[0];
            AutoFilter autofilter1 = sheet.AutoFilter;

            autofilter1.Range = &quot;A1:B1&quot;;
            autofilter1.Filter(0, &quot;A&quot;);
            autofilter1.Refresh();
            sheet.Cells.HideRow(1);
            wb.Save(Constants.destPath +&quot;filteredBook2.xls&quot;);
            wb = new Workbook(Constants.destPath + &quot;filteredBook2.xls&quot;);
            Assert.AreEqual(0.0, wb.Worksheets[0].Cells.GetRowHeight(1));
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


