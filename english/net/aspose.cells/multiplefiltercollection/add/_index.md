---
title: MultipleFilterCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: MultipleFilterCollection method. Adds string filter
type: docs
url: /net/aspose.cells/multiplefiltercollection/add/
---
## MultipleFilterCollection.Add method

Adds string filter.

```csharp
public void Add(string filter)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filter | String | The filter data. |

### Examples

```csharp
// Called: mfc.Add("abc");
public void MultipleFilterCollection_Method_Add()
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

* class [MultipleFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


