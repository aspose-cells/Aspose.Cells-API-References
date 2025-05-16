---
title: SettableChartGlobalizationSettings.SetChartTitleName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Sets the name of Chart Title
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/setcharttitlename/
---
## SettableChartGlobalizationSettings.SetChartTitleName method

Sets the name of Chart Title.

```csharp
public void SetChartTitleName(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | local dependent name |

### Examples

```csharp
namespace AsposeCellsExamples.SettableChartGlobalizationSettingsMethodSetChartTitleNameWithStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetChartTitleNameWithStringDemo
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
                // Call SetChartTitleName with custom title
                settings.SetChartTitleName("Custom Chart Title");

                // Apply settings to workbook - no cast needed since SettableChartGlobalizationSettings should inherit from GlobalizationSettings
                workbook.Settings.GlobalizationSettings = settings;

                // Set chart title (this will use the globalization settings)
                chart.Title.Text = "Chart Title";

                Console.WriteLine("SetChartTitleName method executed successfully with parameter (\"Custom Chart Title\")");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetChartTitleName method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodSetChartTitleNameDemo.xlsx");
        }
    }

    // Define SettableChartGlobalizationSettings class that inherits from GlobalizationSettings
    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string _chartTitleName;

        public void SetChartTitleName(string name)
        {
            _chartTitleName = name;
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


