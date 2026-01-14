---
title: Slicer.Shape
second_title: Aspose.Cells for .NET API Reference
description: Slicer property. Returns the Shape object associated with the specified slicer. Readonly
type: docs
url: /net/aspose.cells.slicers/slicer/shape/
---
## Slicer.Shape property

Returns the Shape object associated with the specified slicer. Read-only.

```csharp
public SlicerShape Shape { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slicers;
    using Aspose.Cells.Pivot;
    using System;

    public class SlicerPropertyShapeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Add a slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            try
            {
                // Access the Shape property (read-only)
                var slicerShape = slicer.Shape;

                // Display information about the Shape
                Console.WriteLine("Slicer Shape Type: " + slicerShape.GetType().Name);
                Console.WriteLine("Slicer Shape Name: " + slicerShape.Name);
                Console.WriteLine("Slicer Shape Width: " + slicerShape.Width);
                Console.WriteLine("Slicer Shape Height: " + slicerShape.Height);

                // Save the workbook
                workbook.Save("SlicerShapeDemo.xlsx");
                Console.WriteLine("Slicer Shape has been demonstrated and saved.");
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

* class [SlicerShape](../../../aspose.cells.drawing/slicershape/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


