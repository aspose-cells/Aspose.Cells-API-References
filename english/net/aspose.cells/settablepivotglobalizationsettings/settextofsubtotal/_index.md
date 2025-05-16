---
title: SettablePivotGlobalizationSettings.SetTextOfSubTotal
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text of PivotFieldSubtotalType type in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofsubtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfSubTotal method

Sets the text of [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) type in the PivotTable.

```csharp
public void SetTextOfSubTotal(PivotFieldSubtotalType subTotalType, string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | The [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |
| text | String | The text of given type |

### Examples

```csharp
namespace AsposeCellsExamples.SettablePivotGlobalizationSettingsMethodSetTextOfSubTotalWithPivotFieldSubtotalTypeStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfSubTotalWithPivotFieldSubtotalTypeStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["A4"].Value = "Food";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 800;
            worksheet.Cells["B4"].Value = 1200;

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Call SetTextOfSubTotal method to change subtotal labels
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum");
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Average");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("SetTextOfSubTotal method executed successfully with parameters (PivotFieldSubtotalType, String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfSubTotal method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfSubTotalDemo.xlsx");
        }
    }

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        private string _sumText = "Sum";
        private string _averageText = "Average";

        public void SetTextOfSubTotal(PivotFieldSubtotalType subTotalType, string text)
        {
            switch (subTotalType)
            {
                case PivotFieldSubtotalType.Sum:
                    _sumText = text;
                    break;
                case PivotFieldSubtotalType.Average:
                    _averageText = text;
                    break;
            }
        }

        public string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
        {
            return subTotalType switch
            {
                PivotFieldSubtotalType.Sum => _sumText,
                PivotFieldSubtotalType.Average => _averageText,
                _ => string.Empty
            };
        }
    }
}
```

### See Also

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


