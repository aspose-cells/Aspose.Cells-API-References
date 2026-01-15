---
title: SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the the text of the value area field header in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader method

Sets the the text of the value area field header in the PivotTable.

```csharp
public void SetTextOfDataFieldHeader(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of data field header name |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfDataFieldHeaderWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // Create an instance of SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Set custom text for the data field header
                settings.SetTextOfDataFieldHeader("Custom Data Header");

                // Verify the change by getting the current text
                string currentHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Data field header text: {currentHeaderText}");

                // Save the workbook to demonstrate successful execution
                workbook.Save("SetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("SetTextOfDataFieldHeader method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


