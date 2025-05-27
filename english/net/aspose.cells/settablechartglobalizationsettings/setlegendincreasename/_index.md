---
title: SettableChartGlobalizationSettings.SetLegendIncreaseName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Sets the name of increase for Legend
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/setlegendincreasename/
---
## SettableChartGlobalizationSettings.SetLegendIncreaseName method

Sets the name of increase for Legend.

```csharp
public void SetLegendIncreaseName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetLegendIncreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Month");
            worksheet.Cells["A2"].PutValue("Jan");
            worksheet.Cells["A3"].PutValue("Feb");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1800);
            
            // Create a column chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Create and configure globalization settings
            var settings = new SettableChartGlobalizationSettings();
            
            try
            {
                // Call SetLegendIncreaseName with custom increase name
                settings.SetLegendIncreaseName("Growth");
                
                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;
                
                // Enable legend
                chart.Legend.Position = LegendPositionType.Bottom;
                
                Console.WriteLine("SetLegendIncreaseName method executed successfully with parameter (\"Growth\")");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLegendIncreaseName method: {ex.Message}");
            }
            
            // Save the workbook
            workbook.Save("MethodSetLegendIncreaseNameDemo.xlsx");
        }
    }

    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string legendIncreaseName;

        public void SetLegendIncreaseName(string name)
        {
            legendIncreaseName = name;
        }

        public string GetLegendIncreaseName()
        {
            return legendIncreaseName;
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


