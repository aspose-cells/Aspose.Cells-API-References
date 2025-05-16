---
title: SettableChartGlobalizationSettings.GetAxisUnitName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Gets the Name of Axis Unit
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/getaxisunitname/
---
## SettableChartGlobalizationSettings.GetAxisUnitName method

Gets the Name of Axis Unit.

```csharp
public override string GetAxisUnitName(DisplayUnitType type)
```

### Examples

```csharp
namespace AsposeCellsExamples.SettableChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
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
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            
            // Create a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Set display units for value axis
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            
            // Create globalization settings
            var settings = new SettableChartGlobalizationSettings();
            
            try
            {
                // Call GetAxisUnitName with DisplayUnitType.Millions
                string unitName = settings.GetAxisUnitName(DisplayUnitType.Millions);
                
                // Set custom unit name
                settings.SetAxisUnitName(DisplayUnitType.Millions, "Mio");
                
                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;
                
                Console.WriteLine($"Original unit name: {unitName}");
                Console.WriteLine("Custom unit name set for Millions display unit");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetAxisUnitName method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("MethodGetAxisUnitNameDemo.xlsx");
        }
    }

    public class SettableChartGlobalizationSettings : GlobalizationSettings
    {
        private string _axisUnitName;

        public string GetAxisUnitName(DisplayUnitType type)
        {
            return _axisUnitName ?? type.ToString();
        }

        public void SetAxisUnitName(DisplayUnitType type, string name)
        {
            _axisUnitName = name;
        }
    }
}
```

### See Also

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


