---
title: SettableChartGlobalizationSettings.GetAxisTitleName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Gets the name of Title for Axis
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/getaxistitlename/
---
## SettableChartGlobalizationSettings.GetAxisTitleName method

Gets the name of Title for Axis.

```csharp
public override string GetAxisTitleName()
```

### Examples

```csharp
namespace AsposeCellsExamples.SettableChartGlobalizationSettingsMethodGetAxisTitleNameDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Create globalization settings
            var globalizationSettings = new SettableChartGlobalizationSettings();
            globalizationSettings.SetAxisTitleName("Custom Axis Title");

            // Apply globalization settings to workbook
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            try
            {
                // Get the axis title name
                string axisTitleName = globalizationSettings.GetAxisTitleName();
                Console.WriteLine($"Axis Title Name: {axisTitleName}");

                // Set axis title - using correct property names from the Chart class definition
                chart.CategoryAxis.Title.Text = axisTitleName;
                chart.ValueAxis.Title.Text = axisTitleName;

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetAxisTitleName method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodGetAxisTitleNameDemo.xlsx");
        }
    }

    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string axisTitleName;

        public void SetAxisTitleName(string name)
        {
            axisTitleName = name;
        }

        public string GetAxisTitleName()
        {
            return axisTitleName;
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


