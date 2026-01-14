---
title: GlobalizationSettings.GetMultipleItemsName
second_title: Aspose.Cells for .NET API Reference
description: GlobalizationSettings method. Gets the name of the Multiple Items label in the PivotTable
type: docs
url: /net/aspose.cells/globalizationsettings/getmultipleitemsname/
---
## GlobalizationSettings.GetMultipleItemsName method

Gets the name of the "(Multiple Items)" label in the PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfMultipleItems() method instead.")]
public virtual string GetMultipleItemsName()
```

### Return Value

The name of "(Multiple Items)" label

### Remarks

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetMultipleItemsNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepare sample data for PivotTable
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Create PivotTable
            int pivotIndex = worksheet.PivotTables.Add("D1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Configure PivotField to show multiple items
            PivotField rowField = pivotTable.RowFields[0];
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.HideItem(0, false); // Select "A"
            rowField.HideItem(1, false); // Select "B"

            // Initialize globalization settings
            GlobalizationSettings gSettings = workbook.Settings.GlobalizationSettings ?? new GlobalizationSettings();
            workbook.Settings.GlobalizationSettings = gSettings;

            try
            {
                // Call GetMultipleItemsName and display result
                string multipleItemsName = gSettings.GetMultipleItemsName();
                Console.WriteLine($"Multiple Items Name: {multipleItemsName}");

                // Refresh PivotTable to apply settings
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetMultipleItemsName: {ex.Message}");
            }

            // Save the workbook to show PivotTable with multiple items label
            workbook.Save("GlobalizationSettingsMethodGetMultipleItemsNameDemo.xlsx");
        }
    }
}
```

### See Also

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


