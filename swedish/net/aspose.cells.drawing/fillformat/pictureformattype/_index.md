---
title: "FillFormat.PictureFormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Hämtar och anger bildformatstypen"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/pictureformattype/
---
## FillFormat.PictureFormatType property

Hämtar och anger bildformattypen.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera bildfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Ange bildfyllningsegenskaper
            shape.Fill.Type = FillType.Texture;
            shape.Fill.Texture = TextureType.BlueTissuePaper;
            shape.Fill.PictureFormatType = FillPictureType.Stretch;

            // Spara arbetsboken
            workbook.Save("FillFormatPictureTypeDemo.xlsx");

            // Läs in den sparade arbetsboken för att verifiera egenskaperna
            Workbook verifyWorkbook = new Workbook("FillFormatPictureTypeDemo.xlsx");
            Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];

            // Skriv ut PictureFormatType för att demonstrera dess användning
            Console.WriteLine("PictureFormatType: " + verifyShape.Fill.PictureFormatType);
        }
    }
}
```

### Se även

* enum [FillPictureType](../../fillpicturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


