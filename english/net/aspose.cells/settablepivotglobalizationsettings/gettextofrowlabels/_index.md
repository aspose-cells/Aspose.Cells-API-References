---
title: SettablePivotGlobalizationSettings.GetTextOfRowLabels
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text of Row Labels label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/gettextofrowlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfRowLabels method

Gets the text of "Row Labels" label in the PivotTable.

```csharp
public override string GetTextOfRowLabels()
```

### Return Value

The text of row labels

### Examples

```csharp
namespace AsposeCellsExamples.SettablePivotGlobalizationSettings
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string rowLabelsText = "Row Labels"; // Default value

        public string GetTextOfRowLabels()
        {
            return rowLabelsText;
        }

        public void SetTextOfRowLabels(string text)
        {
            rowLabelsText = text;
        }
    }

    public class SettablePivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["B2"].Value = "Apple";
            worksheet.Cells["B3"].Value = "Carrot";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 800;

            // Create pivot table
            var pivotIndex = worksheet.PivotTables.Add("A1:C3", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Get default "Row Labels" text
                string defaultRowLabelsText = settings.GetTextOfRowLabels();
                Console.WriteLine($"Default row labels text: {defaultRowLabelsText}");

                // Set custom text for row labels
                settings.SetTextOfRowLabels("Custom Row Headers");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;

                // Refresh pivot table to apply changes
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("GetTextOfRowLabels and SetTextOfRowLabels methods executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing methods: {ex.Message}");
            }

            // Save the result
            workbook.Save("SettablePivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo.xlsx");
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


