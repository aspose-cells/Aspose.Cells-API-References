---
title: PivotField.InsertBlankRow
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether to insert a blank line after each item
type: docs
url: /net/aspose.cells.pivot/pivotfield/insertblankrow/
---
## PivotField.InsertBlankRow property

Indicates whether to insert a blank line after each item.

```csharp
public bool InsertBlankRow { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyInsertBlankRowDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add sample data
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B4"].Value = 20;
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B5"].Value = 5;
            sheet.Cells["A6"].Value = "Orange";
            sheet.Cells["B6"].Value = 8;
            
            // Create pivot table
            int index = sheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Add row field and data field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Set InsertBlankRow property
            PivotField rowField = pivotTable.RowFields[0];
            rowField.InsertBlankRow = true;
            
            // Refresh and calculate pivot table
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Save the workbook
            workbook.Save("PivotFieldInsertBlankRowDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


