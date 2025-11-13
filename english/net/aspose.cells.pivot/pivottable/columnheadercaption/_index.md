---
title: PivotTable.ColumnHeaderCaption
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the custom Caption of the Column Header of the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/columnheadercaption/
---
## PivotTable.ColumnHeaderCaption property

Gets and sets the custom Caption of the Column Header of the PivotTable.

```csharp
public string ColumnHeaderCaption { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnHeaderCaptionDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Quarter";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bike";
            cells["A3"].Value = "Bike";
            cells["A4"].Value = "Car";
            cells["A5"].Value = "Car";
            
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q1";
            cells["B5"].Value = "Q2";
            
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;
            cells["C5"].Value = 4000;

            // Add a pivot table
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Add fields to areas
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Quarter
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
            
            // Set column header caption
            PivotField columnField = pivotTable.ColumnFields[0];
            pivotTable.ColumnHeaderCaption = "Quarter Header";
            
            // Save the workbook
            workbook.Save("PivotTableColumnHeaderCaptionDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


