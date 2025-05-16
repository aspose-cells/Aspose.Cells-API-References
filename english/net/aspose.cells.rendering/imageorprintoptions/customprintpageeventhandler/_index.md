---
title: ImageOrPrintOptions.CustomPrintPageEventHandler
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Client can special output to printer when print each page using this EventHandler
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/
---
## ImageOrPrintOptions.CustomPrintPageEventHandler property

Client can special output to printer when print each page using this EventHandler

```csharp
public PrintPageEventHandler CustomPrintPageEventHandler { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ImageOrPrintOptionsPropertyCustomPrintPageEventHandlerDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;

    public class ImageOrPrintOptionsPropertyCustomPrintPageEventHandlerDemo
    {
        private class CustomDrawHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                HandlePrintPageEvent(drawObject, x, y, width, height);
            }
        }

        public static void Run()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data that will be rendered
            worksheet.Cells["A1"].PutValue("Aspose.Cells CustomPrintPageEventHandler Demo");
            worksheet.Cells["A2"].PutValue("This text will be rendered with custom page settings");

            // Create ImageOrPrintOptions instance
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;

            // Display initial handler state
            Console.WriteLine("Initial DrawObjectEventHandler: " + 
                (options.DrawObjectEventHandler == null ? "Not Assigned" : "Assigned"));

            // Assign custom print handler
            options.DrawObjectEventHandler = new CustomDrawHandler();

            // Verify assignment
            Console.WriteLine("After assignment: " + 
                (options.DrawObjectEventHandler == null ? "Not Assigned" : "Assigned"));

            // Render worksheet to PNG to trigger events
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output.png");

            Console.WriteLine("Rendered image with custom handler settings.");
        }

        private static void HandlePrintPageEvent(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Demonstrate accessing draw object properties
            Console.WriteLine($"Rendering {drawObject.Type} at position ({x},{y})");
            
            // Example modification: Add red border around cells
            if (drawObject.Type == DrawObjectEnum.Cell)
            {
                // Implementation for setting red border would go here
                // Actual API doesn't contain SetBorderRed method in DrawObject
            }
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


