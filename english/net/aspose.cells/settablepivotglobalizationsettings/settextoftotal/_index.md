---
title: SettablePivotGlobalizationSettings.SetTextOfTotal
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text of Total label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextoftotal/
---
## SettablePivotGlobalizationSettings.SetTextOfTotal method

Sets the text of "Total" label in the PivotTable.

```csharp
public void SetTextOfTotal(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfTotalWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data for context
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = 200;

            // Create an instance of SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Get the default "Total" text
                string defaultTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Default Total text: {defaultTotalText}");

                // Set a custom text for "Total"
                settings.SetTextOfTotal("Custom Total Label");

                // Verify the change
                string updatedTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Updated Total text: {updatedTotalText}");

                // Save the workbook
                workbook.Save("SetTextOfTotalDemo.xlsx");
                Console.WriteLine("SetTextOfTotal method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


