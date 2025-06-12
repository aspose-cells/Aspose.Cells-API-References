---
title: SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the the text of the value area field header in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/gettextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader method

Gets the the text of the value area field header in the PivotTable.

```csharp
public override string GetTextOfDataFieldHeader()
```

### Return Value

The text of data field header name

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfDataFieldHeaderDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create sample data for pivot table
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = "North";
            cells["C4"].Value = 3000;

            // Create pivot table
            var pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2);

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();
            
            try
            {
                // Get and display the default text of data field header
                string defaultText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Default data field header text: {defaultText}");

                // Change the data field header text
                settings.SetTextOfDataFieldHeader("Custom Data Header");
                
                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings as GlobalizationSettings;

                // Refresh pivot table to apply changes
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Data field header text changed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfDataFieldHeader method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("MethodGetTextOfDataFieldHeaderDemo.xlsx");
        }
    }

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string _dataFieldHeaderText = "Sum";

        public string GetTextOfDataFieldHeader()
        {
            return _dataFieldHeaderText;
        }

        public void SetTextOfDataFieldHeader(string text)
        {
            _dataFieldHeaderText = text;
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


