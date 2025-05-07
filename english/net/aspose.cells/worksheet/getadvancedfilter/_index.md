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
            var workbook = new Workbook(Constants.sourcePath + "CELLSNET55531.xlsx");
            var sheet = workbook.Worksheets["TEST2"];
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            Assert.AreEqual("A2:K41", filter.ListRange);
            Assert.AreEqual("N8:O10", filter.CriteriaRange);
            Assert.AreEqual("N16:X16", filter.CopyToRange);
        }
```

### See Also

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


