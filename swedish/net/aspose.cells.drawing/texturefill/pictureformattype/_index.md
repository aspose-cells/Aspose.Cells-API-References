---
title: "TextureFill.PictureFormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextureFill-egenskap. Hämtar och anger bildformatstypen"
type: docs
url: /sv/net/aspose.cells.drawing/texturefill/pictureformattype/
---
## TextureFill.PictureFormatType property

Hämtar och anger bildformattypen.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Ställ in fyllningstyp till textur
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;

            // Läs in minimal 1x1‑pixel PNG-bild (vit)
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            textureFill.ImageData = Convert.FromBase64String(base64Image);

            // Visa aktuell PictureFormatType
            Console.WriteLine("Initial PictureFormatType: " + textureFill.PictureFormatType);

            // Ändra till staplat format och aktivera tilening
            textureFill.PictureFormatType = FillPictureType.Stack;
            textureFill.IsTiling = true;

            // Lägg till en annan form för att jämföra det ursprungliga utdragna formatet
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 210, 0, 100, 200);
            shape2.Fill.FillType = FillType.Texture;
            TextureFill textureFill2 = shape2.Fill.TextureFill;
            textureFill2.ImageData = Convert.FromBase64String(base64Image);

            // Spara arbetsboken med båda texturfyllningsexemplen
            workbook.Save("TextureFillPictureFormatTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FillPictureType](../../fillpicturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


