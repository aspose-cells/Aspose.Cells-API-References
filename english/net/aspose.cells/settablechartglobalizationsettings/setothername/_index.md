---
title: SettableChartGlobalizationSettings.SetOtherName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Sets the name of Other labels for Chart
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/setothername/
---
## SettableChartGlobalizationSettings.SetOtherName method

Sets the name of "Other" labels for Chart.

```csharp
public void SetOtherName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetOtherNameWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Group 1");
            worksheet.Cells["A3"].PutValue("Group 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Create a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Create and configure globalization settings
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // Call SetOtherName with a custom label
                settings.SetOtherName("Custom Other Label");
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetOtherName method called successfully with parameter: \"Custom Other Label\"");
                
                // Save the workbook
                workbook.Save("SetOtherNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOtherName: {ex.Message}");
            }
        }
    }

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


