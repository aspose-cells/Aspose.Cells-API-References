---
title: SettablePivotGlobalizationSettings.SetTextOfProtectedName
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text for specific protected name
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofprotectedname/
---
## SettablePivotGlobalizationSettings.SetTextOfProtectedName method

Sets the text for specific protected name.

```csharp
public void SetTextOfProtectedName(string protectedName, string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | String | The protected name in PivotTable. |
| text | String | The local prorected names of PivotTable. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data for context
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Create an instance of SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Set custom text for a protected name
                settings.SetTextOfProtectedName("Sum", "Custom Sum Label");

                // Verify the change by getting the current text
                string currentText = settings.GetTextOfProtectedName("Sum");
                Console.WriteLine($"Text for protected name 'Sum': {currentText}");

                // Save the workbook to demonstrate successful execution
                workbook.Save("SetTextOfProtectedNameDemo.xlsx");
                Console.WriteLine("SetTextOfProtectedName method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


