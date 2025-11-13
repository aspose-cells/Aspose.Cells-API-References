---
title: PivotField.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the display name of pivot field in the pivot table view
type: docs
url: /net/aspose.cells.pivot/pivotfield/displayname/
---
## PivotField.DisplayName property

Represents the display name of pivot field in the pivot table view.

```csharp
public string DisplayName { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Create a workbook and add sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Create pivot table
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Add row field and data field
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Set custom display name for the data field
            pivotTable.DataFields[0].DisplayName = "Total Sales";
            
            // Refresh and calculate pivot table
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Access cell using display name
            Cell cell = pivotTable.GetCellByDisplayName("Total Sales");
            Console.WriteLine("Cell found at row: {0}, column: {1}", cell.Row, cell.Column);
            
            // Save the workbook
            workbook.Save("PivotFieldDisplayNameDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


