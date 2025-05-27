---
title: SettableChartGlobalizationSettings.GetLegendDecreaseName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Gets the name of Decrease for Legend
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/
---
## SettableChartGlobalizationSettings.GetLegendDecreaseName method

Gets the name of Decrease for Legend.

```csharp
public override string GetLegendDecreaseName()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Jan");
            worksheet.Cells["A3"].PutValue("Feb");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(800);

            // Add a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Create and configure globalization settings
            var settings = new SettableChartGlobalizationSettings();
            settings.SetLegendDecreaseName("Custom Decrease");

            // Apply settings to workbook
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Get the legend decrease name
                string decreaseName = settings.GetLegendDecreaseName();
                Console.WriteLine($"Legend Decrease Name: {decreaseName}");

                // Set the legend position
                chart.Legend.Position = LegendPositionType.Right;

                Console.WriteLine("GetLegendDecreaseName method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLegendDecreaseName method: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("MethodGetLegendDecreaseNameDemo.xlsx");
        }
    }

    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string legendDecreaseName;

        public void SetLegendDecreaseName(string name)
        {
            legendDecreaseName = name;
        }

        public string GetLegendDecreaseName()
        {
            return legendDecreaseName;
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


