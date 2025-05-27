---
title: SettableChartGlobalizationSettings.SetAxisUnitName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Sets the Name of Axis Unit
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/setaxisunitname/
---
## SettableChartGlobalizationSettings.SetAxisUnitName method

Sets the Name of Axis Unit.

```csharp
public void SetAxisUnitName(DisplayUnitType type, string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | DisplayUnitType | The unit type for displaying axis labels. |
| name | String | local dependent name |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetAxisUnitNameWithDisplayUnitTypeStringDemo
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
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200000);
            worksheet.Cells["B3"].PutValue(1500000);
            worksheet.Cells["B4"].PutValue(1800000);
            worksheet.Cells["B5"].PutValue(2100000);

            // Create a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Set display units for value axis
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            chart.ValueAxis.DisplayUnitLabel.Text = "Millions"; // Set text directly instead of using IsVisible

            // Create globalization settings
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // Call SetAxisUnitName with DisplayUnitType and custom name
                settings.SetAxisUnitName(DisplayUnitType.Millions, "Millions (Custom)");

                // Apply settings to workbook (instead of chart)
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetAxisUnitName method executed successfully with parameters (DisplayUnitType.Millions, \"Millions (Custom)\")");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetAxisUnitName method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodSetAxisUnitNameDemo.xlsx");
        }
    }

    // Add this class definition if it doesn't exist
    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        public void SetAxisUnitName(DisplayUnitType displayUnit, string name)
        {
            // Implementation would go here
        }
    }
}
```

### See Also

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


