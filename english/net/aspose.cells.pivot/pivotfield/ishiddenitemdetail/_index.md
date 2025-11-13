---
title: PivotField.IsHiddenItemDetail
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Gets whether to hide the detail of the specific PivotItem
type: docs
url: /net/aspose.cells.pivot/pivotfield/ishiddenitemdetail/
---
## PivotField.IsHiddenItemDetail method

Gets whether to hide the detail of the specific PivotItem..

```csharp
public bool IsHiddenItemDetail(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the pivotItem in the pivotField. |

### Return Value

whether the specific PivotItem is hidden detail

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemDetailWithInt32Demo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Country";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Japan";
            cells["A3"].Value = "Japan";
            cells["A4"].Value = "USA";
            cells["A5"].Value = "USA";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;
            cells["B5"].Value = 4000;

            // Add pivot table
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Get pivot field
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Hide item detail for index 1 (USA)
            pivotField.HideItemDetail(1, true);
            
            // Refresh and calculate pivot table
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Check if item detail is hidden
            Console.WriteLine("Is item at index 1 hidden? " + pivotField.IsHiddenItemDetail(1));
            
            // Save workbook
            workbook.Save("PivotFieldIsHiddenItemDetailDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


