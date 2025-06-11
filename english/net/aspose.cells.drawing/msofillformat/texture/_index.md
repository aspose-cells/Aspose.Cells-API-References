---
title: MsoFillFormat.Texture
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat property. Gets the texture fill type
type: docs
url: /net/aspose.cells.drawing/msofillformat/texture/
---
## MsoFillFormat.Texture property

Gets the texture fill type.

```csharp
public TextureType Texture { get; }
```

### Examples

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyTextureDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape sourceShape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 300);
            sourceShape.Fill.Texture = TextureType.BlueTissuePaper;

            Shape destShape = worksheet.Shapes.AddRectangle(0, 4, 100, 200, 300, 400);
            destShape.Fill.Texture = sourceShape.Fill.Texture;

            Console.WriteLine($"Source texture: {sourceShape.Fill.Texture}");
            Console.WriteLine($"Destination texture: {destShape.Fill.Texture}");

            workbook.Save("TextureDemoOutput.xlsx");
        }
    }
}
```

### See Also

* enum [TextureType](../../texturetype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


