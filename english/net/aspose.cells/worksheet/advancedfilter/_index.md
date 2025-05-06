---
title: Worksheet.AdvancedFilter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Filters data using complex criteria
type: docs
url: /net/aspose.cells/worksheet/advancedfilter/
---
## Worksheet.AdvancedFilter method

Filters data using complex criteria.

```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo, 
    bool uniqueRecordOnly)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isFilter | Boolean | Indicates whether filtering the list in place. |
| listRange | String | The list range. |
| criteriaRange | String | The criteria range. |
| copyTo | String | The range where copying data to. |
| uniqueRecordOnly | Boolean | Only displaying or copying unique rows. |

### Examples

```csharp
// Called: sheet.AdvancedFilter(false, &amp;quot;A2:K41&amp;quot;, &amp;quot;N8:O10&amp;quot;, &amp;quot;N16:X57&amp;quot;, false);
[Test]
        public void Method_Boolean_()
        {
            var workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET55530.xlsx&quot;);
            var sheet = workbook.Worksheets[&quot;TEST2&quot;];

            //Even after changing the area, it still doesn&apos;t work
            //sheet.AdvancedFilter(false, &quot;A2:K41&quot;, &quot;N8:O10&quot;, &quot;N16:X16&quot;, false);
            sheet.AdvancedFilter(false, &quot;A2:K41&quot;, &quot;N8:O10&quot;, &quot;N16:X57&quot;, false);
            Assert.AreEqual(&quot;94&quot;, sheet.Cells[&quot;R17&quot;].StringValue);
            Assert.AreEqual(&quot;2023037&quot;, sheet.Cells[&quot;N25&quot;].StringValue);
            workbook.Save(Constants.destPath + &quot;CELLSNET55530.xlsx&quot;);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


