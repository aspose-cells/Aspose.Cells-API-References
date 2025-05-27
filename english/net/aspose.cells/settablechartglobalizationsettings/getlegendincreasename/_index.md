---
title: SettableChartGlobalizationSettings.GetLegendIncreaseName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Gets the name of increase for Legend
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/getlegendincreasename/
---
## SettableChartGlobalizationSettings.GetLegendIncreaseName method

Gets the name of increase for Legend.

```csharp
public override string GetLegendIncreaseName()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Create a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Create and configure globalization settings
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();
            settings.SetLegendIncreaseName("Custom Increase Label");
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Get the current legend increase name
                string increaseName = settings.GetLegendIncreaseName();
                Console.WriteLine($"Current legend increase name: {increaseName}");

                // Save the workbook
                workbook.Save("MethodGetLegendIncreaseNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLegendIncreaseName method: {ex.Message}");
            }
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


