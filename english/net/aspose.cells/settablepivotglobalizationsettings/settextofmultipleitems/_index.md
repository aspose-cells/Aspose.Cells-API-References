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
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfMultipleItemsWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Create pivot table
            var pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Call SetTextOfMultipleItems method to change "(Multiple Items)" text
                settings.SetTextOfMultipleItems("Selected Items");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings as GlobalizationSettings;
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;

                Console.WriteLine("SetTextOfMultipleItems method executed successfully. Changed '(Multiple Items)' to 'Selected Items'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfMultipleItems method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfMultipleItemsDemo.xlsx");
        }
    }

    // Define SettablePivotGlobalizationSettings class that inherits from GlobalizationSettings
    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string _multipleItemsText = "(Multiple Items)";

        public void SetTextOfMultipleItems(string text)
        {
            _multipleItemsText = text;
        }

        public string GetTextOfMultipleItems()
        {
            return _multipleItemsText;
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


