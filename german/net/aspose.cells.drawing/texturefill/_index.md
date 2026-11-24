---
title: "Klasse TextureFill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.TextureFill Klasse. Kapselt das Objekt, das das Texturfüllformat darstellt"
type: docs
url: /de/net/aspose.cells.drawing/texturefill/
---
## TextureFill class

Kapselt das Objekt, das das Format einer Texturfüllung darstellt

```csharp
public class TextureFill : Fill
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ImageData](../../aspose.cells.drawing/texturefill/imagedata/) { get; set; } | Liest und setzt die Bilddaten der Füllung. |
| [IsTiling](../../aspose.cells.drawing/texturefill/istiling/) { get; set; } | Gibt an, ob das Bild als Textur gekachelt wird. |
| [PicFormatOption](../../aspose.cells.drawing/texturefill/picformatoption/) { get; set; } | Liest oder setzt die Bildformatoption. |
| [PictureFormatType](../../aspose.cells.drawing/texturefill/pictureformattype/) { get; set; } | Liest und setzt den Bildformattyp. |
| [Scale](../../aspose.cells.drawing/texturefill/scale/) { get; set; } | Liest und setzt die Bildformatskalierung. |
| [TilePicOption](../../aspose.cells.drawing/texturefill/tilepicoption/) { get; set; } | Liest oder setzt die Kachelbildoption. |
| [Transparency](../../aspose.cells.drawing/texturefill/transparency/) { get; set; } | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [Type](../../aspose.cells.drawing/texturefill/type/) { get; set; } | Liest und setzt den Texturtyp |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Geerbt von [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Liest den Hash‑Code. (Geerbt von [`Fill`](../fill/).) |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge eine Rechteckform hinzu, um die Texturfüllung zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 150, 300);
            
            // Wende Texturfüllung auf die Form an und erhalte die vorhandene TextureFill‑Instanz
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;
            
            // Setze den integrierten Texturtyp
            textureFill.Type = TextureType.BlueTissuePaper;
            
            // Kachelungsoptionen konfigurieren
            textureFill.IsTiling = true;
            TilePicOption tileOptions = new TilePicOption
            {
                ScaleX = 0.5,
                ScaleY = 0.5,
                OffsetX = 10,
                OffsetY = 10
            };
            textureFill.TilePicOption = tileOptions;
            
            // Setze Fülltransparenz und Skalierung
            textureFill.Transparency = 0.2;
            textureFill.Scale = 0.8;
            
            // Speichere die Arbeitsmappe mit angewandter Texturfüllung
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


