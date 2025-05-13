---
title: ChartGlobalizationSettings.GetLegendIncreaseName
second_title: Aspose.Cells for .NET API Reference
description: ChartGlobalizationSettings method. Gets the name of increase for Legend
type: docs
url: /net/aspose.cells.charts/chartglobalizationsettings/getlegendincreasename/
---
## ChartGlobalizationSettings.GetLegendIncreaseName method

Gets the name of increase for Legend.

```csharp
public virtual string GetLegendIncreaseName()
```

### Examples

```csharp
// Called: string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();
public static void ChartGlobalizationSettings_Method_GetLegendIncreaseName()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a sample chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Create an instance of ChartGlobalizationSettings
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();

            // Demonstrate the usage of methods in ChartGlobalizationSettings
            string seriesName = globalizationSettings.GetSeriesName();
            string chartTitleName = globalizationSettings.GetChartTitleName();
            string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();
            string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();
            string legendTotalName = globalizationSettings.GetLegendTotalName();
            string axisTitleName = globalizationSettings.GetAxisTitleName();
            string otherName = globalizationSettings.GetOtherName();
            string axisUnitName = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);

            // Print the retrieved names to the console
            Console.WriteLine("Series Name: " + seriesName);
            Console.WriteLine("Chart Title Name: " + chartTitleName);
            Console.WriteLine("Legend Increase Name: " + legendIncreaseName);
            Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);
            Console.WriteLine("Legend Total Name: " + legendTotalName);
            Console.WriteLine("Axis Title Name: " + axisTitleName);
            Console.WriteLine("Other Name: " + otherName);
            Console.WriteLine("Axis Unit Name: " + axisUnitName);

            // Save the workbook
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
            workbook.Save("ChartGlobalizationSettingsExample.pdf");
        }
```

### See Also

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


