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
    using System;

    public class SettableChartGlobalizationSettingsMethodSetOtherNameWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add minimal data for context
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(150);

            try
            {
                // Create an instance of SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Set a custom name for the "Other" label
                settings.SetOtherName("Miscellaneous Items");

                // Verify the setting by getting the value
                string otherName = settings.GetOtherName();
                Console.WriteLine("Other Name set to: " + otherName);

                // Save the workbook
                workbook.Save("SetOtherNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOtherName: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


