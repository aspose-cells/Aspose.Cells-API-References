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
// Called: MultipleFilterCollection mfc = new MultipleFilterCollection();
public void Cells_Type_MultipleFilterCollection()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    cells[1, 0].PutValue("abc");
    cells[2, 0].PutValue("def");
    cells[5, 0].PutValue("ghi");
    cells[10, 0].PutValue("abc");

    FilterColumn fc = sheet.AutoFilter.FilterColumns[0];
    fc.FilterType = FilterType.MultipleFilters;
    MultipleFilterCollection mfc = new MultipleFilterCollection();

    mfc.Add("abc");
    mfc.Add("ghi");
    mfc.MatchBlank = false;
    fc.Filter = mfc;

    sheet.AutoFilter.Refresh();
    for (int i = 1; i < 11; i++)
    {
        Assert.AreEqual(i != 1 && i != 5 && i != 10, cells.IsRowHidden(i),
            "Row[" + i + "].IsHidden");
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


