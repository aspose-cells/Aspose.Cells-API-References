---
title: PivotItem.Index
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Gets the index of the pivot item in cache field
type: docs
url: /net/aspose.cells.pivot/pivotitem/index/
---
## PivotItem.Index property

Gets the index of the pivot item in cache field.

```csharp
[Obsolete("Use PivotItem.Position property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Index { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotItem.Position property . This method will be removed 6 months later since August 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIndexDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            
            // Create pivot table
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Get the row field
            PivotField rowField = pivotTable.RowFields[0];
            
            // Access pivot items using Index property
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Item: {item.Value}, Index: {item.Index}");
                
                // Hide item detail using Index property
                if (item.Value.ToString() == "Apple")
                {
                    rowField.HideItemDetail(item.Index, true);
                }
            }
            
            // Calculate and refresh pivot table
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Save the workbook
            workbook.Save("PivotItemPropertyIndexDemo_out.xlsx");
        }
    }
}
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


