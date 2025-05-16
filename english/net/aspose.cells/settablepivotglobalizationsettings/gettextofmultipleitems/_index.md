---
title: SettablePivotGlobalizationSettings.GetTextOfMultipleItems
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text of Multiple Items label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/gettextofmultipleitems/
---
## SettablePivotGlobalizationSettings.GetTextOfMultipleItems method

Gets the text of "(Multiple Items)" label in the PivotTable.

```csharp
public override string GetTextOfMultipleItems()
```

### Return Value

The text of "(Multiple Items)" label

### Examples

```csharp
namespace AsposeCellsExamples.SettablePivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Fruits";
            worksheet.Cells["B2"].Value = "Apple";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Fruits";
            worksheet.Cells["B3"].Value = "Orange";
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Vegetables";
            worksheet.Cells["B4"].Value = "Carrot";
            worksheet.Cells["C4"].Value = 1500;

            // Create pivot table
            var pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Get the default text for multiple items
                string defaultText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Default text for multiple items: {defaultText}");

                // Set custom text for multiple items
                settings.SetTextOfMultipleItems("Custom Multiple Items Text");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings as GlobalizationSettings;

                // Refresh pivot table to apply changes
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("GetTextOfMultipleItems method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfMultipleItems method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodGetTextOfMultipleItemsDemo.xlsx");
        }
    }

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string _multipleItemsText = "(Multiple Items)";

        public string GetTextOfMultipleItems()
        {
            return _multipleItemsText;
        }

        public void SetTextOfMultipleItems(string text)
        {
            _multipleItemsText = text;
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


