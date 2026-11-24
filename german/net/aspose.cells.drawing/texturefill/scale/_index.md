---
title: "TextureFill.Scale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextureFill-Eigenschaft. Ruft die Skalierung des Bildformats ab und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/texturefill/scale/
---
## TextureFill.Scale property

Liest und setzt die Bildformatskalierung.

```csharp
public double Scale { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TextureFillPropertyScaleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form hinzufügen und ihr Füllformat abrufen
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 500, 300);
            FillFormat fillFormat = shape.Fill;

            // Texturfüllung konfigurieren
            fillFormat.FillType = FillType.Texture;
            TextureFill textureFill = fillFormat.TextureFill;

            // Texturbild laden und Eigenschaften konfigurieren
            textureFill.ImageData = File.ReadAllBytes("texture.jpg");
            textureFill.Type = TextureType.Unknown; // Changed from UserDefined to Unknown
            textureFill.IsTiling = true;

            // Skalierung anzeigen und ändern
            Console.WriteLine("Initial Scale: " + textureFill.Scale);
            textureFill.Scale = 0.5;
            Console.WriteLine("Modified Scale: " + textureFill.Scale);

            // Ergebnis speichern
            workbook.Save("TextureFillScaleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


