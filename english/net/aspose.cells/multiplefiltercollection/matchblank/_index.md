---
title: MultipleFilterCollection.MatchBlank
second_title: Aspose.Cells for .NET API Reference
description: MultipleFilterCollection property. Indicates whether to filter by blank
type: docs
url: /net/aspose.cells/multiplefiltercollection/matchblank/
---
## MultipleFilterCollection.MatchBlank property

Indicates whether to filter by blank.

```csharp
public bool MatchBlank { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(multiFilters.MatchBlank);
public void MultipleFilterCollection_Property_MatchBlank()
{
    var wb = new Workbook(Constants.sourcePath + "example.xlsx");
    var ws = wb.Worksheets["Sheet1"];
    var autoFilter = ws.AutoFilter;

        

    autoFilter.AddFilter(0, null);
    autoFilter.AddFilter(0, "");
    autoFilter.Refresh();
    Assert.AreEqual(FilterType.MultipleFilters, autoFilter.FilterColumns[0].FilterType);
    MultipleFilterCollection multiFilters = (MultipleFilterCollection)autoFilter.FilterColumns[0].Filter;
    Assert.IsTrue(multiFilters.MatchBlank);
}
```

### See Also

* class [MultipleFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


