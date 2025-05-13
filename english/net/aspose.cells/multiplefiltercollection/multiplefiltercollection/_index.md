---
title: MultipleFilterCollection.MultipleFilterCollection
second_title: Aspose.Cells for .NET API Reference
description: MultipleFilterCollection constructor. Constructs one new instance
type: docs
url: /net/aspose.cells/multiplefiltercollection/multiplefiltercollection/
---
## MultipleFilterCollection constructor

Constructs one new instance.

```csharp
public MultipleFilterCollection()
```

### Examples

```csharp
// Called: MultipleFilterCollection mfc = new MultipleFilterCollection();
public void MultipleFilterCollection_Constructor()
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


