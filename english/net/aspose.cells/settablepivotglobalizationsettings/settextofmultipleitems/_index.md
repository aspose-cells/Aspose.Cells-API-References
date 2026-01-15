---
title: SettablePivotGlobalizationSettings.SetTextOfMultipleItems
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text of Multiple Items label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofmultipleitems/
---
## SettablePivotGlobalizationSettings.SetTextOfMultipleItems method

Sets the text of "(Multiple Items)" label in the PivotTable.

```csharp
public void SetTextOfMultipleItems(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfMultipleItemsWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data (optional, just for context)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Create an instance of SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Set custom text for the "(Multiple Items)" label in a PivotTable
                settings.SetTextOfMultipleItems("(Multiple Items Edited)");

                // Retrieve and display the updated text
                string currentText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Current text of '(Multiple Items)' label: {currentText}");

                // (Optional) Save the workbook – no pivot table is required for this demo
                workbook.Save("SetTextOfMultipleItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


