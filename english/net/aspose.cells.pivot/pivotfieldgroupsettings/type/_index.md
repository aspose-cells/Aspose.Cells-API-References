---
title: PivotFieldGroupSettings.Type
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldGroupSettings property. Gets the group type of pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfieldgroupsettings/type/
---
## PivotFieldGroupSettings.Type property

Gets the group type of pivot field.

```csharp
public virtual PivotFieldGroupType Type { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsPropertyTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            worksheet.Cells["A3"].Value = new DateTime(2023, 1, 2);
            worksheet.Cells["A4"].Value = new DateTime(2023, 1, 3);

            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // Add a pivot table to the worksheet
                int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "D3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Add fields to the pivot table
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

                // Access the row field and group by date
                PivotField rowField = pivotTable.RowFields[0];
                rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("DateGroup", new int[] { 0, 1 }) }, true);

                // Access the group settings of the row field
                PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

                // Display the current value of the Type property (read-only)
                Console.WriteLine("Pivot Field Group Type: " + groupSettings.Type);

                // Save the workbook
                workbook.Save("PivotFieldGroupSettingsTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotFieldGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


