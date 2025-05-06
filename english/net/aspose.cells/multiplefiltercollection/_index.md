---
title: Class MultipleFilterCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.MultipleFilterCollection class. Represents the multiple filter collection
type: docs
url: /net/aspose.cells/multiplefiltercollection/
---
## MultipleFilterCollection class

Represents the multiple filter collection.

```csharp
public class MultipleFilterCollection : CollectionBase
```

## Constructors

| Name | Description |
| --- | --- |
| [MultipleFilterCollection](multiplefiltercollection/)() | Constructs one new instance. |

## Properties

| Name | Description |
| --- | --- |
| [Item](../../aspose.cells/multiplefiltercollection/item/) { get; } | DateTimeGroupItem or a simple object. |
| [MatchBlank](../../aspose.cells/multiplefiltercollection/matchblank/) { get; set; } | Indicates whether to filter by blank. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/multiplefiltercollection/add/)(string) | Adds string filter. |

### Examples

```csharp
// Called: MultipleFilterCollection multiFilters = (MultipleFilterCollection)autoFilter.FilterColumns[0].Filter;
[Test]
        public void Type_MultipleFilterCollection()
        {
            var wb = new Workbook(Constants.sourcePath + &quot;CellsNet55063.xlsx&quot;);
            var ws = wb.Worksheets[&quot;Sheet1&quot;];
            var autoFilter = ws.AutoFilter;

        

            autoFilter.AddFilter(0, null);
            autoFilter.AddFilter(0, &quot;&quot;);
            autoFilter.Refresh();
            Assert.AreEqual(FilterType.MultipleFilters, autoFilter.FilterColumns[0].FilterType);
            MultipleFilterCollection multiFilters = (MultipleFilterCollection)autoFilter.FilterColumns[0].Filter;
            Assert.IsTrue(multiFilters.MatchBlank);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


