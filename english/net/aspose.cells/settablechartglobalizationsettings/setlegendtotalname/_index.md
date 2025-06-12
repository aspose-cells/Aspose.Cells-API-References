---
title: SettableChartGlobalizationSettings.SetLegendTotalName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Sets the name of Total for Legend
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/setlegendtotalname/
---
## SettableChartGlobalizationSettings.SetLegendTotalName method

Sets the name of Total for Legend.

```csharp
public void SetLegendTotalName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetLegendTotalNameWithStringDemo
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

            // Create globalization settings
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // Call SetLegendTotalName with custom legend total name
                settings.SetLegendTotalName("Custom Total Legend");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetLegendTotalName method executed successfully with parameter (\"Custom Total Legend\")");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLegendTotalName method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodSetLegendTotalNameDemo.xlsx");
        }
    }

    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string _legendTotalName;

        public void SetLegendTotalName(string name)
        {
            _legendTotalName = name;
        }

        public string GetLegendTotalName()
        {
            return _legendTotalName;
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


