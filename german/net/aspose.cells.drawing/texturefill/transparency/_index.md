---
title: "TextureFill.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextureFill-Eigenschaft. Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0.0 (undurchsichtig) bis 1.0 (klar)"
type: docs
url: /de/net/aspose.cells.drawing/texturefill/transparency/
---
## TextureFill.Transparency property

Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck-Shape zum Arbeitsblatt hinzu
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Setze den Fülltyp auf Textur
            shape.Fill.FillType = FillType.Texture;

            // Auf die TextureFill-Eigenschaften zugreifen
            TextureFill textureFill = shape.Fill.TextureFill;

            // Einen integrierten Texturtyp festlegen
            textureFill.Type = TextureType.BlueTissuePaper;

            // Anfangstransparenzwert anzeigen
            Console.WriteLine("Initial Transparency: " + textureFill.Transparency);

            // Transparenz auf 70% ändern (0.0 = undurchsichtig, 1.0 = vollständig transparent)
            textureFill.Transparency = 0.7;
            Console.WriteLine("Updated Transparency: " + textureFill.Transparency);

            // Arbeitsmappe mit sichtbarem Transparenzeffekt speichern
            workbook.Save("TextureFillTransparencyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


