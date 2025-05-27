---
title: DrawObject.Cell
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates the Cell object when rendering. All properties of cell can be accessed
type: docs
url: /net/aspose.cells.rendering/drawobject/cell/
---
## DrawObject.Cell property

Indicates the Cell object when rendering. All properties of cell can be accessed.

```csharp
public Cell Cell { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class DrawObjectPropertyCellDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to cell A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Cell Value");

            // Create a text box shape linked to the cell
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.LinkedCell = "A1";

            // Create a draw object through rendering (as DrawObject properties are read-only)
            // Simulate a DrawObject by passing required parameters to the method
            DrawObject_Property_Cell(null, 10, 10, 200, 50, cell, textBox);
        }

        public static void DrawObject_Property_Cell(DrawObject drawObject, float x, float y, float width, float height, Cell cell, Shape shape)
        {
            Console.WriteLine($"Drawing object at X: {x}, Y: {y}, Width: {width}, Height: {height}");
            
            if (cell != null)
            {
                Console.WriteLine($"Rendering Cell: {cell.Name}, Value: {cell.StringValue}");
            }

            if (shape != null)
            {
                Console.WriteLine($"Rendering Shape: {shape.Name}");
            }
        }
    }
}
```

### See Also

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


