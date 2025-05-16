---
title: SettablePivotGlobalizationSettings.SetTextOfRowLabels
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text of Row Labels label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofrowlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfRowLabels method

Sets the text of "Row Labels" label in the PivotTable.

```csharp
public void SetTextOfRowLabels(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of row labels |

### Examples

```csharp
namespace AsposeCellsExamples.SettablePivotGlobalizationSettingsMethodSetTextOfRowLabelsWithStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfRowLabelsWithStringDemo
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
                // Call SetTextOfRowLabels method to change "Row Labels" text
                settings.SetTextOfRowLabels("Categories");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("SetTextOfRowLabels method executed successfully. Changed 'Row Labels' to 'Categories'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfRowLabels method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfRowLabelsDemo.xlsx");
        }
    }

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string _rowLabelsText = "Row Labels";

        public string GetTextOfRowLabels()
        {
            return _rowLabelsText;
        }

        public void SetTextOfRowLabels(string text)
        {
            _rowLabelsText = text;
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


