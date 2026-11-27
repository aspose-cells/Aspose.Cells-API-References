---
title: "Klass TextureFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.TextureFill-klass. Inkapslar objektet som representerar formatet för texturfyllning"
type: docs
url: /sv/net/aspose.cells.drawing/texturefill/
---
## TextureFill class

Inkapslar objektet som representerar texturfyllningsformat

```csharp
public class TextureFill : Fill
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ImageData](../../aspose.cells.drawing/texturefill/imagedata/) { get; set; } | Hämtar och anger bilddata för fyllningen. |
| [IsTiling](../../aspose.cells.drawing/texturefill/istiling/) { get; set; } | Anger om bilden ska tileas som textur. |
| [PicFormatOption](../../aspose.cells.drawing/texturefill/picformatoption/) { get; set; } | Hämtar eller anger bildformatalternativ. |
| [PictureFormatType](../../aspose.cells.drawing/texturefill/pictureformattype/) { get; set; } | Hämtar och anger bildformattypen. |
| [Scale](../../aspose.cells.drawing/texturefill/scale/) { get; set; } | Hämtar och anger skalan för bildformatet. |
| [TilePicOption](../../aspose.cells.drawing/texturefill/tilepicoption/) { get; set; } | Hämtar eller anger alternativ för tile-bild. |
| [Transparency](../../aspose.cells.drawing/texturefill/transparency/) { get; set; } | Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar). |
| [Type](../../aspose.cells.drawing/texturefill/type/) { get; set; } | Hämtar och anger texturtypen |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Arv från [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Hämtar hashkoden.(Arv från [`Fill`](../fill/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassTextureFillDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en rektangelform för att demonstrera texturfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 150, 300);
            
            // Applicera texturfyllning på formen och hämta befintlig TextureFill-instans
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;
            
            // Ange inbyggd texturtyp
            textureFill.Type = TextureType.BlueTissuePaper;
            
            // Konfigurera tile-alternativ
            textureFill.IsTiling = true;
            TilePicOption tileOptions = new TilePicOption
            {
                ScaleX = 0.5,
                ScaleY = 0.5,
                OffsetX = 10,
                OffsetY = 10
            };
            textureFill.TilePicOption = tileOptions;
            
            // Ange fyllningens transparens och skalning
            textureFill.Transparency = 0.2;
            textureFill.Scale = 0.8;
            
            // Spara arbetsboken med applicerad texturfyllning
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


