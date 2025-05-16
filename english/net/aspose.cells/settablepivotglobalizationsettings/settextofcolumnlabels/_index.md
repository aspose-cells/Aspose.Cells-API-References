---
title: SettablePivotGlobalizationSettings.SetTextOfColumnLabels
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text of Column Labels label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfColumnLabels method

Gets the text of "Column Labels" label in the PivotTable.

```csharp
public void SetTextOfColumnLabels(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of column labels |

### Examples

```csharp
namespace AsposeCellsExamples.SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsWithStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(2500);
            worksheet.Cells["B3"].PutValue(1800);

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Call SetTextOfColumnLabels method to change "Column Labels" text
                settings.SetTextOfColumnLabels("Regions");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("SetTextOfColumnLabels method executed successfully. Changed 'Column Labels' to 'Regions'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfColumnLabels method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsDemo.xlsx");
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


