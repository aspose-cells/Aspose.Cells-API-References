---
title: SettablePivotGlobalizationSettings.GetTextOfColumnLabels
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text of Column Labels label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/gettextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfColumnLabels method

Gets the text of "Column Labels" label in the PivotTable.

```csharp
public override string GetTextOfColumnLabels()
```

### Return Value

The text of column labels

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfColumnLabelsDemo
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
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Create pivot table
            var pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Get the default text of column labels
                string defaultText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Default column labels text: {defaultText}");

                // Change the column labels text
                settings.SetTextOfColumnLabels("Custom Column Header");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;

                // Refresh pivot table to apply changes
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Column labels text changed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfColumnLabels method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodGetTextOfColumnLabelsDemo.xlsx");
        }
    }

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string _columnLabelsText = "Column Labels";

        public string GetTextOfColumnLabels()
        {
            return _columnLabelsText;
        }

        public void SetTextOfColumnLabels(string text)
        {
            _columnLabelsText = text;
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


