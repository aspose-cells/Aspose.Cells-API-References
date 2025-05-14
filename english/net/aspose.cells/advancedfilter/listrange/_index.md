---
title: AdvancedFilter.ListRange
second_title: Aspose.Cells for .NET API Reference
description: AdvancedFilter property. Gets the list range of this advanced filter
type: docs
url: /net/aspose.cells/advancedfilter/listrange/
---
## AdvancedFilter.ListRange property

Gets the list range of this advanced filter.

```csharp
public string ListRange { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("A2:K41", filter.ListRange);
public void AdvancedFilter_Property_ListRange()
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


