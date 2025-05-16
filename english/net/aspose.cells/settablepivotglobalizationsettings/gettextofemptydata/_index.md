---
title: SettablePivotGlobalizationSettings.GetTextOfEmptyData
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text of blank label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/gettextofemptydata/
---
## SettablePivotGlobalizationSettings.GetTextOfEmptyData method

Gets the text of "(blank)" label in the PivotTable.

```csharp
public override string GetTextOfEmptyData()
```

### Return Value

The text of empty data

### Examples

```csharp
namespace AsposeCellsExamples.SettablePivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data with empty cells for pivot table
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(null);

            // Create pivot table
            var pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Get default text for empty data
                string defaultEmptyText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Default empty data text: {defaultEmptyText}");

                // Set custom text for empty data
                settings.SetTextOfEmptyData("N/A");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;

                // Refresh pivot table to apply changes
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("GetTextOfEmptyData method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfEmptyData method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodGetTextOfEmptyDataDemo.xlsx");
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


