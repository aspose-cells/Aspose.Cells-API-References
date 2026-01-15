---
title: SettableChartGlobalizationSettings.GetLegendIncreaseName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Gets the name of increase for Legend
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/getlegendincreasename/
---
## SettableChartGlobalizationSettings.GetLegendIncreaseName method

Gets the name of increase for Legend.

```csharp
public override string GetLegendIncreaseName()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add minimal data for context
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Create an instance of SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Set a custom legend increase name
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Get the legend increase name using GetLegendIncreaseName
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name: " + legendIncreaseName);

                // Save the workbook
                workbook.Save("GetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


