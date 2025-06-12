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
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfDataFieldHeaderWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Call SetTextOfDataFieldHeader method to change data field header text
                settings.SetTextOfDataFieldHeader("Custom Data Header");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("SetTextOfDataFieldHeader method executed successfully. Changed data field header to 'Custom Data Header'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfDataFieldHeader method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfDataFieldHeaderDemo.xlsx");
        }
    }

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string _dataFieldHeaderText = "Sum";

        public void SetTextOfDataFieldHeader(string text)
        {
            _dataFieldHeaderText = text;
        }

        public string GetTextOfDataFieldHeader()
        {
            return _dataFieldHeaderText;
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


