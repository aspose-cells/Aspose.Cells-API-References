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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    // Custom handler to capture DrawObject events and read the Cell property
    public class CellInfoDrawHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Output basic draw object information
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");

            // Demonstrate reading the read‑only Cell property
            if (drawObject.Cell != null)
            {
                var cell = drawObject.Cell;
                Console.WriteLine($"Cell Name: {cell.Name}");
                Console.WriteLine($"Cell Value: {cell.Value}");
                Console.WriteLine($"Cell Row: {cell.Row}, Column: {cell.Column}");
            }
        }
    }

    public class DrawObjectPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook and get the first worksheet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Add some sample data to cells
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Add a shape to ensure shape draw events are also raised
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Set up rendering options with our custom draw handler
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CellInfoDrawHandler()
                };

                // Render the worksheet – this will trigger the DrawObject events
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectCellDemo.png");

                // Save the workbook (optional)
                workbook.Save("DrawObjectCellDemo.xlsx");
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

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


