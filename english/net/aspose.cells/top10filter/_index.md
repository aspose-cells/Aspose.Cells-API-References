---
title: Class Top10Filter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Top10Filter class. Represents the top 10 filter
type: docs
url: /net/aspose.cells/top10filter/
---
## Top10Filter class

Represents the top 10 filter.

```csharp
public class Top10Filter
```

## Properties

| Name | Description |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } |  |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | Indicates whether the items is percent. |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | Indicates whether it's top filter. |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | Gets and sets the items of the filter. |

### Examples

```csharp
// Called: Top10Filter f = worksheet.AutoFilter.FilterColumns[5].Filter as Top10Filter;
[Test]
        public void Type_Top10Filter()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/N46267.xlsx");
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


