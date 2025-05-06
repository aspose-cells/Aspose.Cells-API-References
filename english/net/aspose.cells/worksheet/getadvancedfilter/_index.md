---
title: Worksheet.GetAdvancedFilter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Gets the settings of advanced filter
type: docs
url: /net/aspose.cells/worksheet/getadvancedfilter/
---
## Worksheet.GetAdvancedFilter method

Gets the settings of advanced filter.

```csharp
public AdvancedFilter GetAdvancedFilter()
```

### Examples

```csharp
// Called: AdvancedFilter filter = sheet.GetAdvancedFilter();
[Test]
        public void Method_GetAdvancedFilter()
        {
            var workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET55531.xlsx&quot;);
            var sheet = workbook.Worksheets[&quot;TEST2&quot;];
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            Assert.AreEqual(&quot;A2:K41&quot;, filter.ListRange);
            Assert.AreEqual(&quot;N8:O10&quot;, filter.CriteriaRange);
            Assert.AreEqual(&quot;N16:X16&quot;, filter.CopyToRange);
        }
```

### See Also

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


