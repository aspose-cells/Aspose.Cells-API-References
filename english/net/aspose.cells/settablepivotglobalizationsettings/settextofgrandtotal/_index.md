---
title: SettablePivotGlobalizationSettings.SetTextOfGrandTotal
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text of Grand Total label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofgrandtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfGrandTotal method

Sets the text of "Grand Total" label in the PivotTable.

```csharp
public void SetTextOfGrandTotal(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |

### Examples

```csharp
namespace AsposeCellsExamples.SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalWithStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalWithStringDemo
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
                // Call SetTextOfGrandTotal method to change "Grand Total" text
                settings.SetTextOfGrandTotal("Custom Grand Total");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("SetTextOfGrandTotal method executed successfully. Changed 'Grand Total' to 'Custom Grand Total'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfGrandTotal method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalDemo.xlsx");
        }
    }

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string _grandTotalText = "Grand Total";

        public void SetTextOfGrandTotal(string text)
        {
            _grandTotalText = text;
        }

        public string GetTextOfGrandTotal()
        {
            return _grandTotalText;
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


