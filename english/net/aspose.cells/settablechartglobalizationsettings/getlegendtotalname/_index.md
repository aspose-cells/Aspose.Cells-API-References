---
title: SettableChartGlobalizationSettings.GetLegendTotalName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Gets the name of Total for Legend
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/getlegendtotalname/
---
## SettableChartGlobalizationSettings.GetLegendTotalName method

Gets the name of Total for Legend.

```csharp
public override string GetLegendTotalName()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendTotalNameDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Create a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Create and configure globalization settings
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();
            settings.SetLegendTotalName("Custom Total Label");
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Get the current legend total name
                string totalName = settings.GetLegendTotalName();
                Console.WriteLine($"Current legend total name: {totalName}");

                // Save the workbook
                workbook.Save("MethodGetLegendTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLegendTotalName method: {ex.Message}");
            }
        }
    }

    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string legendTotalName;

        public void SetLegendTotalName(string name)
        {
            legendTotalName = name;
        }

        public string GetLegendTotalName()
        {
            return legendTotalName;
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


