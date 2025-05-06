---
title: ImageOrPrintOptions.DrawObjectEventHandler
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Implements this interface to get DrawObject and Bound when rendering
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/
---
## ImageOrPrintOptions.DrawObjectEventHandler property

Implements this interface to get DrawObject and Bound when rendering.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Examples

```csharp
// Called: DrawObjectEventHandler = drawObjectEventHandler,
public static void Property_DrawObjectEventHandler()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;World&quot;);
            sheet.Cells[&quot;A3&quot;].Formula = &quot;=A1 &amp; \&quot; \&quot; &amp; A2&quot;;

            // Add a shape
            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddShape(Aspose.Cells.Drawing.MsoDrawingType.Rectangle, 5, 0, 5, 0, 100, 100);
            shape.Text = &quot;Sample Shape&quot;;

            // Create an instance of CustomDrawObjectEventHandler
            CustomDrawObjectEventHandler drawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Set image or print options
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                DrawObjectEventHandler = drawObjectEventHandler,
                OnePagePerSheet = true,
                ImageType = Aspose.Cells.Drawing.ImageType.Png
            };

            // Render the sheet to an image
            SheetRender sr = new SheetRender(sheet, options);
            sr.ToImage(0, &quot;DrawObjectDemo.png&quot;);

            // Save the workbook
            workbook.Save(&quot;DrawObjectDemo.xlsx&quot;);
            workbook.Save(&quot;DrawObjectDemo.pdf&quot;);
        }
```

### See Also

* class [DrawObjectEventHandler](../../drawobjecteventhandler/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


