---
title: "TilePicOption.OffsetX"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TilePicOption-Eigenschaft. Liest oder setzt den X‑Versatz für das Kachelbild"
type: docs
url: /de/net/aspose.cells.drawing/tilepicoption/offsetx/
---
## TilePicOption.OffsetX property

Liest oder setzt den X‑Versatz für das Kachelbild.

```csharp
public double OffsetX { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TilePicOptionPropertyOffsetXDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform hinzu, um das Kacheln zu demonstrieren
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Konfiguriere das Füllformat, um ein Kachelbild zu verwenden
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Erstellen und konfigurieren Sie TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Lese den initialen OffsetX‑Wert
            Console.WriteLine("Current OffsetX value: " + tileOptions.OffsetX);

            // Setze einen neuen X‑Versatz für das Kachelmuster
            tileOptions.OffsetX = 15.5;

            // Wende Kacheloptionen auf die Formfüllung an
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Lade ein minimales 1 × 1‑Pixel‑Bild (roter Punkt)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Modifizierte Arbeitsmappe speichern
            workbook.Save("TilePicOptionPropertyOffsetXDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


