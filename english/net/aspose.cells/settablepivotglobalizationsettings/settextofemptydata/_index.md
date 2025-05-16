---
title: SettablePivotGlobalizationSettings.SetTextOfEmptyData
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text of blank label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofemptydata/
---
## SettablePivotGlobalizationSettings.SetTextOfEmptyData method

Sets the text of "(blank)" label in the PivotTable.

```csharp
public void SetTextOfEmptyData(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of empty data |

### Examples

```csharp
namespace AsposeCellsExamples.SettablePivotGlobalizationSettingsMethodSetTextOfEmptyDataWithStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfEmptyDataWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table with empty cells
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            // B4 intentionally left empty

            // Create pivot table
            var pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Call SetTextOfEmptyData method to change "(blank)" text
                settings.SetTextOfEmptyData("No Data Available");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings as GlobalizationSettings;

                // Refresh pivot table to apply changes
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("SetTextOfEmptyData method executed successfully. Changed '(blank)' to 'No Data Available'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfEmptyData method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfEmptyDataDemo.xlsx");
        }
    }

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string _emptyDataText = "(blank)";

        public string GetTextOfEmptyData()
        {
            return _emptyDataText;
        }

        public void SetTextOfEmptyData(string text)
        {
            _emptyDataText = text;
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


