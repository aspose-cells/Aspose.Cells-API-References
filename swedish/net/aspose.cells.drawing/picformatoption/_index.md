---
title: "Klass PicFormatOption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.PicFormatOption-klass. Representerar bildformatalternativ."
type: docs
url: /sv/net/aspose.cells.drawing/picformatoption/
---
## PicFormatOption class

Representerar bildformatalternativ

```csharp
public class PicFormatOption
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PicFormatOption](picformatoption/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Bottom](../../aspose.cells.drawing/picformatoption/bottom/) { get; set; } | Hämtar eller anger det nedre offsetet för att sträcka bilden. |
| [Left](../../aspose.cells.drawing/picformatoption/left/) { get; set; } | Hämtar eller anger det vänstra offsetet för att sträcka bilden. |
| [Right](../../aspose.cells.drawing/picformatoption/right/) { get; set; } | Hämtar eller anger det högra offsetet för att sträcka bilden. |
| [Scale](../../aspose.cells.drawing/picformatoption/scale/) { get; set; } | Hämtar eller anger hur många bildstackar och skalningsfaktor som används. |
| [Top](../../aspose.cells.drawing/picformatoption/top/) { get; set; } | Hämtar eller anger det övre offsetet för att sträcka bilden. |
| [Type](../../aspose.cells.drawing/picformatoption/type/) { get; set; } | Hämtar eller anger bildens fyllningstyp. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.IO;

    public class DrawingClassPicFormatOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form och ange bildfyllning.
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);
            // FillType-egenskapen har tagits bort från MsoFillFormat-åtkomst.
            shape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");

            // Konfigurera bildformatalternativ.
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.15,
                Right = 0.15,
                Top = 0.15,
                Bottom = 0.15,
                Scale = 0.8
            };

            // Lägg till en andra form med mosaikbild.
            Shape tiledShape = worksheet.Shapes.AddRectangle(5, 210, 0, 0, 200, 200);
            // FillType-egenskapen har tagits bort från MsoFillFormat-åtkomst.
            tiledShape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");
            
            PicFormatOption tileFormat = new PicFormatOption
            {
                Type = FillPictureType.Stack,
                Scale = 1.5
            };

            workbook.Save("PicFormatOptionDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


