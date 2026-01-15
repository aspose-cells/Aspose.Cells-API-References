---
title: GlobalizationSettings.GetPivotGrandTotalName
second_title: Aspose.Cells for .NET API Reference
description: GlobalizationSettings method. Gets the name of the Grand Total label in the PivotTable
type: docs
url: /net/aspose.cells/globalizationsettings/getpivotgrandtotalname/
---
## GlobalizationSettings.GetPivotGrandTotalName method

Gets the name of the "Grand Total" label in the PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfGrandTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotGrandTotalName()
```

### Return Value

The name of "Grand Total" label

### Remarks

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetPivotGrandTotalNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set custom globalization settings
            var settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Populate sample data for pivot table
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Q1";
            cells["C1"].Value = "Q2";
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = 1500;
            cells["C2"].Value = 2200;
            cells["A3"].Value = "Clothing";
            cells["B3"].Value = 900;
            cells["C3"].Value = 1300;

            // Create pivot table with multiple data fields
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C3", "E4");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Q1
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Q2

            // Refresh and calculate pivot table
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            try
            {
                // Demonstrate GetPivotGrandTotalName call
                string grandTotalName = settings.GetPivotGrandTotalName();
                Console.WriteLine($"Custom Grand Total Name: {grandTotalName}");

                // Save modified workbook
                workbook.Save("GlobalizationSettingsMethodGetPivotGrandTotalNameDemo.xlsx");
                Console.WriteLine("Spreadsheet saved. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetPivotGrandTotalName()
            {
                return "[Custom Grand Total]";
            }
        }
    }
}
```

### See Also

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


