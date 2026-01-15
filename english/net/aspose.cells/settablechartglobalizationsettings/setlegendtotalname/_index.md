---
title: SettableChartGlobalizationSettings.SetLegendTotalName
second_title: Aspose.Cells for .NET API Reference
description: SettableChartGlobalizationSettings method. Sets the name of Total for Legend
type: docs
url: /net/aspose.cells/settablechartglobalizationsettings/setlegendtotalname/
---
## SettableChartGlobalizationSettings.SetLegendTotalName method

Sets the name of Total for Legend.

```csharp
public void SetLegendTotalName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetLegendTotalNameWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add minimal data for context
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            try
            {
                // Create an instance of SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Set a custom legend total name
                settings.SetLegendTotalName("Custom Total Label");

                // Verify the setting by getting the value
                string legendTotalName = settings.GetLegendTotalName();
                Console.WriteLine("Legend Total Name set to: " + legendTotalName);

                // Save the workbook
                workbook.Save("SetLegendTotalNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


