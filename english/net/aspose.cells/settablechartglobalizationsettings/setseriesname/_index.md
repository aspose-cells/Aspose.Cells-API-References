---
title: SettableChartGlobalizationSettings.SetSeriesName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Sets the name of Series in the Chart
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/setseriesname/
---
## SettableChartGlobalizationSettings.SetSeriesName method

Sets the name of Series in the Chart.

```csharp
public void SetSeriesName(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | local dependent name |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetSeriesNameWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            
            // Create a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Create globalization settings
            var settings = new SettableChartGlobalizationSettings();
            
            try
            {
                // Call SetSeriesName with custom series name
                settings.SetSeriesName("Custom Series Name");
                
                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;
                
                // Set series name (this will use the globalization settings)
                chart.NSeries[0].Name = "Series Name";
                
                Console.WriteLine("SetSeriesName method executed successfully with parameter (\"Custom Series Name\")");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSeriesName method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("MethodSetSeriesNameDemo.xlsx");
        }
    }

    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string seriesName;

        public void SetSeriesName(string name)
        {
            seriesName = name;
        }

        public string GetSeriesName()
        {
            return seriesName;
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


