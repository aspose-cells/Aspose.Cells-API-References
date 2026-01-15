---
title: SettableChartGlobalizationSettings.SetLegendIncreaseName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Sets the name of increase for Legend
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/setlegendincreasename/
---
## SettableChartGlobalizationSettings.SetLegendIncreaseName method

Sets the name of increase for Legend.

```csharp
public void SetLegendIncreaseName(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | local dependent name |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendIncreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add minimal data for context
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Item 1";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Create an instance of SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Set a custom legend increase name
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Verify the setting by getting the value
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name set to: " + legendIncreaseName);

                // Save the workbook
                workbook.Save("SetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


