---
title: MsoFillFormatHelper.Texture
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper property. Gets the texture fill type
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/texture/
---
## MsoFillFormatHelper.Texture property

Gets the texture fill type.

```csharp
public TextureType Texture { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.MsoFillFormatHelperPropertyTextureDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFillFormatHelperPropertyTextureDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to access MsoFillFormatHelper
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 10, 10, 200, 150);
            MsoFillFormat fillFormat = shape.FillFormat;

            // Set texture fill type by setting image data (since Texture is read-only)
            fillFormat.ImageData = System.IO.File.ReadAllBytes("texture.jpg");

            // Display current texture type
            Console.WriteLine("Current Texture type: " + fillFormat.Texture);

            // Add another shape with different texture for comparison
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 200, 10, 10, 200, 150);
            shape2.FillFormat.ImageData = System.IO.File.ReadAllBytes("canvas.jpg");
            Console.WriteLine("Second shape Texture type: " + shape2.FillFormat.Texture);

            // Save the workbook to demonstrate visual effects
            workbook.Save("TexturePropertyDemo.xlsx");
        }
    }
}
```

### See Also

* enum [TextureType](../../texturetype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


