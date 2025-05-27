---
title: SettablePivotGlobalizationSettings.SetTextOfTotal
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text of Total label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextoftotal/
---
## SettablePivotGlobalizationSettings.SetTextOfTotal method

Sets the text of "Total" label in the PivotTable.

```csharp
public void SetTextOfTotal(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfTotalWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Clothing");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);

            // Create pivot table
            var pivotIndex = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Call SetTextOfTotal method to change "Total" text
                settings.SetTextOfTotal("Custom Total");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings as GlobalizationSettings;
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

                Console.WriteLine("SetTextOfTotal method executed successfully. Changed 'Total' to 'Custom Total'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfTotal method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfTotalDemo.xlsx");
        }
    }

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string _totalText = "Total";

        public void SetTextOfTotal(string text)
        {
            _totalText = text;
        }

        public string GetTextOfTotal()
        {
            return _totalText;
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


