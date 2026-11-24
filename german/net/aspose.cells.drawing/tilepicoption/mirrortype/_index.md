---
title: "TilePicOption.MirrorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TilePicOption-Eigenschaft. Liest oder setzt den Spiegeltyp für das Kacheln"
type: docs
url: /de/net/aspose.cells.drawing/tilepicoption/mirrortype/
---
## TilePicOption.MirrorType property

Liest oder setzt den Spiegeltyp für das Kacheln.

```csharp
public MirrorType MirrorType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyMirrorTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 500, 500, 500);

            // Lade Beispiel-Bilddaten (ersetze durch tatsächlichen Bildpfad)
            byte[] imageData = File.ReadAllBytes("sample.png");

            // Erstelle und konfiguriere eine TilePicOption‑Instanz
            TilePicOption tileOptions = new TilePicOption();

            // Anfangswert von MirrorType anzeigen
            Console.WriteLine("Current MirrorType: " + tileOptions.MirrorType);

            // Kachelungsoptionen konfigurieren
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;
            tileOptions.MirrorType = MirrorType.Both;

            // Kachelkonfiguration mit den korrekten Eigenschaften anwenden
            shape.Fill.FillType = FillType.Texture;
            shape.Fill.ImageData = imageData;
            shape.Fill.TextureFill.TilePicOption = tileOptions;

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("TilePicOptionMirrorTypeDemo.xlsx");

            Console.WriteLine("Updated MirrorType: " + tileOptions.MirrorType);
        }
    }
}
```

### Siehe auch

* enum [MirrorType](../../mirrortype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


