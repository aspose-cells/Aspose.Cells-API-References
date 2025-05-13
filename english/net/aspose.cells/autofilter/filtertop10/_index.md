---
title: AutoFilter.FilterTop10
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Filter the top 10 item in the list
type: docs
url: /net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Filter the top 10 item in the list

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| isTop | Boolean | Indicates whether filter from top or bottom |
| isPercent | Boolean | Indicates whether the items is percent or count |
| itemCount | Int32 | The item count |

### Examples

```csharp
// Called: worksheet.AutoFilter.FilterTop10(5, true, false, 5);
public void AutoFilter_Method_FilterTop10()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    worksheet.AutoFilter.Range = "B6:K10";
    worksheet.AutoFilter.FilterTop10(5, true, false, 5);
    Top10Filter f = worksheet.AutoFilter.FilterColumns[5].Filter as Top10Filter;
    Assert.IsNotNull(f);
    Assert.IsTrue(f.IsTop);
    Assert.IsFalse(f.IsPercent);
    worksheet.AutoFilter.Refresh();
    Cells cells = worksheet.Cells;
    for (int i = 6; i < 30; i++)
    {
        Assert.AreEqual(i != 7 && i != 8 && i != 11 && i != 12 && i != 16,
            cells.IsRowHidden(i), "Row(0 based).Hidden-" + i);
    }
}
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


