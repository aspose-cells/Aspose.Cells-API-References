---
title: SettableChartGlobalizationSettings.GetLegendTotalName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Gets the name of Total for Legend
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/getlegendtotalname/
---
## SettableChartGlobalizationSettings.GetLegendTotalName method

Gets the name of Total for Legend.

```csharp
public override string GetLegendTotalName()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data for context
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Create an instance of SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // First set a custom legend total name
                settings.SetLegendTotalName("Custom Total Label");

                // Call the GetLegendTotalName method to retrieve the value
                string legendTotalName = settings.GetLegendTotalName();

                // Display the result
                Console.WriteLine("Legend Total Name: " + legendTotalName);

                // Save the workbook
                workbook.Save("GetLegendTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


