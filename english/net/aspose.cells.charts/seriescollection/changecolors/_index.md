---
title: SeriesCollection.ChangeColors
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection method. Set Monochromatic Palette for chart series
type: docs
url: /net/aspose.cells.charts/seriescollection/changecolors/
---
## SeriesCollection.ChangeColors method

Set Monochromatic Palette for chart series.

```csharp
public void ChangeColors(ChartColorPaletteType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartColorPaletteType | The Monochromatic Type. |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodChangeColorsWithChartColorPaletDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Populate some data for the chart
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["A2"].PutValue("Jan");
            ws.Cells["A3"].PutValue("Feb");
            ws.Cells["A4"].PutValue("Mar");

            ws.Cells["B1"].PutValue("Series1");
            ws.Cells["B2"].PutValue(10);
            ws.Cells["B3"].PutValue(20);
            ws.Cells["B4"].PutValue(30);

            ws.Cells["C1"].PutValue("Series2");
            ws.Cells["C2"].PutValue(15);
            ws.Cells["C3"].PutValue(25);
            ws.Cells["C4"].PutValue(35);

            // Add a column chart
            int chartIdx = ws.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = ws.Charts[chartIdx];

            // Set the data range for the series
            chart.NSeries.Add("B1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Get the series collection
            SeriesCollection seriesColl = chart.NSeries;

            try
            {
                // Change the color palette of all series in the collection.
                // Use a numeric cast to a valid enum value (e.g., 0) to avoid dependent enum member names.
                seriesColl.ChangeColors((ChartColorPaletteType)0);

                Console.WriteLine("ChangeColors method invoked successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error invoking ChangeColors: {ex.Message}");
            }

            // Save the workbook to verify the result
            workbook.Save("SeriesCollection_ChangeColors_Demo.xlsx");
        }
    }
}
```

### See Also

* enum [ChartColorPaletteType](../../chartcolorpalettetype/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


