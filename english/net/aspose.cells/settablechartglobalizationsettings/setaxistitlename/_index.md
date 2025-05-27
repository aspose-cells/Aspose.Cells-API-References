---
title: SettableChartGlobalizationSettings.SetAxisTitleName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Sets the name of Title for Axis
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/setaxistitlename/
---
## SettableChartGlobalizationSettings.SetAxisTitleName method

Sets the name of Title for Axis.

```csharp
public void SetAxisTitleName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetAxisTitleNameWithStringDemo
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

            // Add axis title
            chart.ValueAxis.Title.Text = "Value Axis";
            chart.CategoryAxis.Title.Text = "Category Axis";

            // Create globalization settings
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // Call SetAxisTitleName with custom axis title name
                settings.SetAxisTitleName("Custom Axis Title");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetAxisTitleName method executed successfully with parameter (\"Custom Axis Title\")");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetAxisTitleName method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodSetAxisTitleNameDemo.xlsx");
        }
    }

    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string _axisTitleName;

        public void SetAxisTitleName(string name)
        {
            _axisTitleName = name;
        }

        public string GetAxisTitleName()
        {
            return _axisTitleName;
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


