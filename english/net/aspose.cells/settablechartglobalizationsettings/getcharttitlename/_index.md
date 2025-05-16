---
title: SettableChartGlobalizationSettings.GetChartTitleName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Gets the name of Chart Title
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/getcharttitlename/
---
## SettableChartGlobalizationSettings.GetChartTitleName method

Gets the name of Chart Title.

```csharp
public override string GetChartTitleName()
```

### Examples

```csharp
namespace AsposeCellsExamples.SettableChartGlobalizationSettingsMethodGetChartTitleNameDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetChartTitleNameDemo
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
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            
            // Create a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Create globalization settings
            var globalizationSettings = new SettableChartGlobalizationSettings();
            
            // Set custom chart title name
            globalizationSettings.SetChartTitleName("Custom Chart Title");
            
            // Apply globalization settings to workbook
            workbook.Settings.GlobalizationSettings = globalizationSettings;
            
            try
            {
                // Get the chart title name
                string chartTitleName = globalizationSettings.GetChartTitleName();
                
                // Set the chart title
                chart.Title.Text = chartTitleName;
                
                Console.WriteLine($"Chart title set to: {chartTitleName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetChartTitleName method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("MethodGetChartTitleNameDemo.xlsx");
        }
    }

    // Add this class definition to make the code compile
    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string chartTitleName;

        public void SetChartTitleName(string name)
        {
            chartTitleName = name;
        }

        public string GetChartTitleName()
        {
            return chartTitleName;
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


