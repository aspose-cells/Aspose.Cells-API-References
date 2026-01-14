---
title: Slicer.ColumnWidth
second_title: Aspose.Cells for .NET API Reference
description: Slicer property. Returns or sets the width of each column in the slicer in unit of points
type: docs
url: /net/aspose.cells.slicers/slicer/columnwidth/
---
## Slicer.ColumnWidth property

Returns or sets the width of each column in the slicer in unit of points.

```csharp
public double ColumnWidth { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyColumnWidthDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            
            // Add pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Add slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Set column width in points
            slicer.ColumnWidth = 80;
            
            // Save the workbook
            workbook.Save("SlicerColumnWidthDemo.xlsx");
        }
    }
}
```

### See Also

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


