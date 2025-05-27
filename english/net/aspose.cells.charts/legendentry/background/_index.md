---
title: LegendEntry.Background
second_title: Aspose.Cells for .NET API Reference
description: LegendEntry property. Gets and sets the display mode of the background
type: docs
url: /net/aspose.cells.charts/legendentry/background/
---
## LegendEntry.Background property

Gets and sets the display mode of the background

```csharp
[Obsolete("Use LegendEntry.BackgroundMode property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use LegendEntry.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyBackgroundDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 10);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            Aspose.Cells.Charts.Legend legend = chart.Legend;
            Aspose.Cells.Charts.LegendEntryCollection legendEntries = legend.LegendEntries;

            if (legendEntries.Count > 0)
            {
                Aspose.Cells.Charts.LegendEntry firstEntry = legendEntries[0];
                firstEntry.BackgroundMode = BackgroundMode.Transparent;
            }

            workbook.Save("LegendEntryBackgroundDemo.xlsx");
        }
    }
}
```

### See Also

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


