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
// Called: Assert.AreEqual("N8:O10", filter.CriteriaRange);
[Test]
        public void Property_CriteriaRange()
        {
            var workbook = new Workbook(Constants.sourcePath + "CELLSNET55531.xlsx");
            var sheet = workbook.Worksheets["TEST2"];
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            Assert.AreEqual("A2:K41", filter.ListRange);
            Assert.AreEqual("N8:O10", filter.CriteriaRange);
            Assert.AreEqual("N16:X16", filter.CopyToRange);
        }
```

### See Also

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


