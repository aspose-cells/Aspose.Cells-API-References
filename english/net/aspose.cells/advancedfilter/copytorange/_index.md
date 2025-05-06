---
title: AdvancedFilter.CopyToRange
second_title: Aspose.Cells for .NET API Reference
description: AdvancedFilter property. Gets the range where copying the resut of this advanced filter to
type: docs
url: /net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

Gets the range where copying the resut of this advanced filter to.

```csharp
public string CopyToRange { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;N16:X16&amp;quot;, filter.CopyToRange);
[Test]
        public void Property_CopyToRange()
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


