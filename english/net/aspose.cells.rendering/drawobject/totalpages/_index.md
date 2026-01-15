---
title: DrawObject.TotalPages
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates total pages in current rendering
type: docs
url: /net/aspose.cells.rendering/drawobject/totalpages/
---
## DrawObject.TotalPages property

Indicates total pages in current rendering.

```csharp
public int TotalPages { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyTotalPagesDemo
    {
        // Custom handler to capture DrawObject events and read the TotalPages property
        private class TotalPagesHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Display the TotalPages property value
                Console.WriteLine($"Total Pages in Rendering: {drawObject.TotalPages}");
                Console.WriteLine($"Current Page: {drawObject.CurrentPage + 1}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Create a new workbook and get the first worksheet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Add sample data to make the rendering meaningful
                sheet.Cells["A1"].PutValue("Sample Data");
                sheet.Cells["A2"].PutValue("More Data");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Add a shape to ensure multiple draw objects are generated
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Set up rendering options with our custom handler
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = false, // Allow multiple pages to demonstrate TotalPages
                    DrawObjectEventHandler = new TotalPagesHandler()
                };

                // Render the worksheet - this will trigger the DrawObject events
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "TotalPagesDemo.png");

                // Save the workbook
                workbook.Save("TotalPagesDemo.xlsx");
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

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


