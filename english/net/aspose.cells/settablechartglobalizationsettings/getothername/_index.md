---
title: SettableChartGlobalizationSettings.GetOtherName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Gets the name of Other labels for Chart
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/getothername/
---
## SettableChartGlobalizationSettings.GetOtherName method

Gets the name of "Other" labels for Chart.

```csharp
public override string GetOtherName()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["A6"].PutValue("Other");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            // Create a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B6", true);
            chart.NSeries.CategoryData = "A2:A6";

            // Create and apply globalization settings
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();
            settings.SetOtherName("Custom Other Label");
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Get the current "Other" label name
                string otherName = settings.GetOtherName();
                Console.WriteLine($"Current 'Other' label name: {otherName}");

                // Save the workbook
                workbook.Save("MethodGetOtherNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOtherName method: {ex.Message}");
            }
        }
    }

    // Define SettableChartGlobalizationSettings class that inherits from GlobalizationSettings
    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string otherName;

        public void SetOtherName(string name)
        {
            otherName = name;
        }

        public string GetOtherName()
        {
            return otherName;
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


