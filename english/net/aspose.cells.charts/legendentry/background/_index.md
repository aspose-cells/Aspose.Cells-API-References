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
// Called: firstEntry.Background = BackgroundMode.Transparent;
public static void Property_Background()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data for the chart
            sheet.Cells[0, 1].PutValue("Income");
            sheet.Cells[1, 0].PutValue("Company A");
            sheet.Cells[2, 0].PutValue("Company B");
            sheet.Cells[3, 0].PutValue("Company C");
            sheet.Cells[1, 1].PutValue(10000);
            sheet.Cells[2, 1].PutValue(20000);
            sheet.Cells[3, 1].PutValue(30000);

            // Add a chart to the worksheet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Access the legend of the chart
            Legend legend = chart.Legend;

            // Access the collection of legend entries
            LegendEntryCollection legendEntries = legend.LegendEntries;

            // Modify properties of the first legend entry
            if (legendEntries.Count > 0)
            {
                LegendEntry firstEntry = legendEntries[0];
                firstEntry.IsDeleted = false;
                firstEntry.AutoScaleFont = true;
                firstEntry.Background = BackgroundMode.Transparent;
            }

            // Save the workbook
            workbook.Save("LegendEntryCollectionExample.xlsx");
            workbook.Save("LegendEntryCollectionExample.pdf");
        }
```

### See Also

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


