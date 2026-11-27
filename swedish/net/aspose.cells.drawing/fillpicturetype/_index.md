---
title: "Enum FillPictureType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.FillPictureType enum. Representerar bildens fyllningstyp"
type: docs
url: /sv/net/aspose.cells.drawing/fillpicturetype/
---
## FillPictureType enumeration

Representerar bildfyllningstypen.

```csharp
public enum FillPictureType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Stretch | `0` | Sträck |
| Stack | `1` | Stapla |
| StackAndScale | `2` | StaplaOchSkala |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFillPictureTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform för att demonstrera bildfyllning
            Shape shape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 200, 200);

            // Ange bildfyllningsegenskaper
            shape.Fill.Type = FillType.Texture;
            shape.Fill.PictureFormatType = FillPictureType.StackAndScale;

            // Använd minimal 1x1‑pixelbild (vit) för demonstration
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            shape.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Lägg till en annan form med annan fyllningstyp
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 5, 2, 0, 200, 200);
            shape2.Fill.Type = FillType.Texture;
            shape2.Fill.PictureFormatType = FillPictureType.Stretch;
            shape2.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Spara arbetsboken med olika fyllningskonfigurationer
            workbook.Save("FillPictureTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


