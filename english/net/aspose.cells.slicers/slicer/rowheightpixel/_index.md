---
title: Slicer.RowHeightPixel
second_title: Aspose.Cells for .NET API Reference
description: Slicer property. Returns or sets the height of each row in the specified slicer in unit of pixels
type: docs
url: /net/aspose.cells.slicers/slicer/rowheightpixel/
---
## Slicer.RowHeightPixel property

Returns or sets the height of each row in the specified slicer, in unit of pixels.

```csharp
public int RowHeightPixel { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyRowHeightPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Create sample data for pivot table
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(40);

            // Create pivot table
            int pivotIndex = workbook.Worksheets[0].PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Add slicer and get reference
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Set slicer properties
            slicer.RowHeightPixel = 30;
            slicer.Width = 150;

            workbook.Save("SlicerRowHeightDemo_output.xlsx");
        }
    }
}
```

### See Also

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


