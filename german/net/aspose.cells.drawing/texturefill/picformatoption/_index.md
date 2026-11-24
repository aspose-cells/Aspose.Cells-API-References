---
title: "TextureFill.PicFormatOption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextureFill-Eigenschaft. Ruft die Bildformatoption ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/texturefill/picformatoption/
---
## TextureFill.PicFormatOption property

Liest oder setzt die Bildformatoption.

```csharp
public PicFormatOption PicFormatOption { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyPicFormatOptionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            var shape = worksheet.Shapes.AddRectangle(0, 0, 100, 300, 200, 400);

            // Texturfüllung konfigurieren
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;

            // Benutzerdefinierte Textur mit minimalem 1x1-Pixel-Bild festlegen
            // TextureType.UserDefined ist nicht verfügbar, die ungültige Zuweisung wurde entfernt
            textureFill.ImageData = new byte[] { 
                0x89, 0x50, 0x4E, 0x47, 0x0D, 0x0A, 0x1A, 0x0A, 0x00, 0x00, 0x00, 0x0D, 0x49, 0x48, 0x44, 0x52,
                0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x08, 0x02, 0x00, 0x00, 0x00, 0x90, 0x77, 0x53,
                0xDE, 0x00, 0x00, 0x00, 0x01, 0x73, 0x52, 0x47, 0x42, 0x00, 0xAE, 0xCE, 0x1C, 0xE9, 0x00, 0x00,
                0x00, 0x04, 0x67, 0x41, 0x4D, 0x41, 0x00, 0x00, 0xB1, 0x8F, 0x0B, 0xFC, 0x61, 0x05, 0x00, 0x00,
                0x00, 0x09, 0x70, 0x48, 0x59, 0x73, 0x00, 0x00, 0x0E, 0xC3, 0x00, 0x00, 0x0E, 0xC3, 0x01, 0xC7,
                0x6F, 0xA8, 0x64, 0x00, 0x00, 0x00, 0x18, 0x49, 0x44, 0x41, 0x54, 0x18, 0x57, 0x63, 0x60, 0x18,
                0x05, 0xA3, 0x60, 0x14, 0x8C, 0x82, 0x51, 0x30, 0x0A, 0x46, 0xC1, 0x28, 0x00, 0x00, 0x01, 0xAD,
                0x00, 0x01, 0x8C, 0xF8, 0x2B, 0xD4, 0x00, 0x00, 0x00, 0x00, 0x49, 0x45, 0x4E, 0x44, 0xAE, 0x42,
                0x60, 0x82 
            };

            // Kachelung aktivieren und Formatoptionen anzeigen
            textureFill.IsTiling = true;

            // Anfänglichen PicFormatOption-Zustand anzeigen
            Console.WriteLine("Initial PicFormatOption: " + (textureFill.PicFormatOption != null ? "Configured" : "Null"));

            // Neue Formatoptionen erstellen und anwenden
            textureFill.PicFormatOption = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Scale = 0.25,
                Left = 15,    // Corrected from LeftOffset
                Top = 15,     // Corrected from TopOffset
                // ScaleX- und ScaleY-Eigenschaften existieren nicht – entfernt
            };

            // Eigenschaftsaktualisierung überprüfen
            Console.WriteLine("Updated PicFormatOption Type: " + textureFill.PicFormatOption.Type);

            // Speichern mit geändertem Kachelmuster
            workbook.Save("TextureFillPicFormatOptionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PicFormatOption](../../picformatoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


