---
title: "Enum MirrorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MirrorType enum. Representerar spegeltyp för texturfyllning"
type: docs
url: /sv/net/aspose.cells.drawing/mirrortype/
---
## MirrorType enumeration

Representerar spegeltyp för texturfyllning.

```csharp
public enum MirrorType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen |
| Horizonal | `1` | Horisontell |
| Vertical | `2` | Vertikal |
| Both | `3` | Båda |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassMirrorTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera MirrorType
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 200);

            // Ställ in texturfyllning med olika spegeltyper
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Horizonal;
            shape = worksheet.Shapes.AddRectangle(2, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Vertical;
            shape = worksheet.Shapes.AddRectangle(3, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Both;
            shape = worksheet.Shapes.AddRectangle(4, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.None;

            // Spara resultatet
            workbook.Save("MirrorTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


