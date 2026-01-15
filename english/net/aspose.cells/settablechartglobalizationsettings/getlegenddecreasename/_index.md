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
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add simple data for context (optional)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Create a chart (optional, just to have a complete workbook)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Instantiate the globalization settings object
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Set a custom legend decrease label
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // Retrieve the label using GetLegendDecreaseName
                string legendDecreaseName = settings.GetLegendDecreaseName();

                Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

                // Save the workbook (the settings are not directly attached to the chart in this demo)
                workbook.Save("GetLegendDecreaseNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLegendDecreaseName: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


