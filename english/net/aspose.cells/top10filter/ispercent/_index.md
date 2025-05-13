---
title: Top10Filter.IsPercent
second_title: Aspose.Cells for .NET API Reference
description: Top10Filter property. Indicates whether the items is percent
type: docs
url: /net/aspose.cells/top10filter/ispercent/
---
## Top10Filter.IsPercent property

Indicates whether the items is percent.

```csharp
public bool IsPercent { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(f.IsPercent);
public void Top10Filter_Property_IsPercent()
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

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


