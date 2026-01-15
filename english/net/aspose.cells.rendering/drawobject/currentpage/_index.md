---
title: DrawObject.CurrentPage
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering
type: docs
url: /net/aspose.cells.rendering/drawobject/currentpage/
---
## DrawObject.CurrentPage property

Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering.

```csharp
public int CurrentPage { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyCurrentPageDemo
    {
        // Custom handler to read and display the CurrentPage property
        private class CurrentPageHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Display the CurrentPage property value
                Console.WriteLine($"CurrentPage: {drawObject.CurrentPage}");
                Console.WriteLine($"TotalPages: {drawObject.TotalPages}");
                Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Create a new workbook and access the first worksheet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add some sample data to make the rendering meaningful
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["A2"].PutValue("More Data");
                worksheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Add a shape to generate shape-type draw objects
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Set up rendering options with our custom draw handler
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CurrentPageHandler()
                };

                // Render the worksheet to trigger DrawObject events
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "CurrentPageDemo.png");

                // Save the workbook
                workbook.Save("CurrentPageDemo.xlsx");
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


