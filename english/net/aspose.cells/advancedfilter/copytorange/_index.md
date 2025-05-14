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
// Called: Assert.AreEqual("N16:X16", filter.CopyToRange);
public void AdvancedFilter_Property_CopyToRange()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
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


