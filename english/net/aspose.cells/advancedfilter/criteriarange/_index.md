---
title: AdvancedFilter.CriteriaRange
second_title: Aspose.Cells for .NET API Reference
description: AdvancedFilter property. Gets the criteria range of this advanced filter
type: docs
url: /net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

Gets the criteria range of this advanced filter.

```csharp
public string CriteriaRange { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;N8:O10&amp;quot;, filter.CriteriaRange);
[Test]
        public void Property_CriteriaRange()
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

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


