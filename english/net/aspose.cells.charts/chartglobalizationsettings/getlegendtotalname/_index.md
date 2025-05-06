---
title: ChartGlobalizationSettings.GetLegendTotalName
second_title: Aspose.Cells for .NET API Reference
description: ChartGlobalizationSettings method. Gets the name of Total for Legend
type: docs
url: /net/aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/
---
## ChartGlobalizationSettings.GetLegendTotalName method

Gets the name of Total for Legend.

```csharp
public virtual string GetLegendTotalName()
```

### Examples

```csharp
// Called: string legendTotalName = globalizationSettings.GetLegendTotalName();
public static void Method_GetLegendTotalName()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a sample chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add sample data for the chart
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category 1&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Category 2&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Category 3&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(10);
            worksheet.Cells[&quot;B2&quot;].PutValue(20);
            worksheet.Cells[&quot;B3&quot;].PutValue(30);

            chart.NSeries.Add(&quot;B1:B3&quot;, true);
            chart.NSeries.CategoryData = &quot;A1:A3&quot;;

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
            Console.WriteLine(&quot;Series Name: &quot; + seriesName);
            Console.WriteLine(&quot;Chart Title Name: &quot; + chartTitleName);
            Console.WriteLine(&quot;Legend Increase Name: &quot; + legendIncreaseName);
            Console.WriteLine(&quot;Legend Decrease Name: &quot; + legendDecreaseName);
            Console.WriteLine(&quot;Legend Total Name: &quot; + legendTotalName);
            Console.WriteLine(&quot;Axis Title Name: &quot; + axisTitleName);
            Console.WriteLine(&quot;Other Name: &quot; + otherName);
            Console.WriteLine(&quot;Axis Unit Name: &quot; + axisUnitName);

            // Save the workbook
            workbook.Save(&quot;ChartGlobalizationSettingsExample.xlsx&quot;);
            workbook.Save(&quot;ChartGlobalizationSettingsExample.pdf&quot;);
        }
```

### See Also

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


