---
title: TextureFill.Type
second_title: Aspose.Cells for .NET API Reference
description: TextureFill property. Gets and sets the texture type
type: docs
url: /net/aspose.cells.drawing/texturefill/type/
---
## TextureFill.Type property

Gets and sets the texture type

```csharp
public TextureType Type { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.TextureFillPropertyTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create a shape with texture fill
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 100, 200, 200);
            shape.Fill.FillType = FillType.Texture;
            
            // Display initial texture type
            Console.WriteLine("Initial Texture Type: " + shape.Fill.Texture);
            
            // Set new texture type and configure tiling
            shape.Fill.Texture = TextureType.BlueTissuePaper;
            shape.Fill.TextureFill.IsTiling = true;
            
            // Create second shape to compare types
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 2, 0, 100, 200, 200);
            shape2.Fill.FillType = FillType.Texture;
            shape2.Fill.Texture = TextureType.WaterDroplets;
            shape2.Fill.TextureFill.IsTiling = true;
            
            // Save with different texture types
            workbook.Save("TextureTypeDemo.xlsx");
            
            Console.WriteLine("Updated Texture Type: " + shape.Fill.Texture);
        }
    }
}
```

### See Also

* enum [TextureType](../../texturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


