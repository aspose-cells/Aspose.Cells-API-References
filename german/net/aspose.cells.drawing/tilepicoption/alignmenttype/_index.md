---
title: "TilePicOption.AlignmentType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TilePicOption-Eigenschaft. Gibt die Ausrichtung für das Kacheln zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/tilepicoption/alignmenttype/
---
## TilePicOption.AlignmentType property

Liest oder setzt die Ausrichtung für das Kacheln.

```csharp
public RectangleAlignmentType AlignmentType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform hinzu, um das Kacheln zu demonstrieren
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 300);

            // Konfiguriere das Füllformat, um ein Kachelbild zu verwenden
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Erstellen und konfigurieren Sie TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Anfangswert von AlignmentType anzeigen
            Console.WriteLine("Current AlignmentType: " + tileOptions.AlignmentType);

            // Ausrichtung auf TopRight setzen
            tileOptions.AlignmentType = RectangleAlignmentType.TopRight;
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;

            // Wende Kacheloptionen auf die Formfüllung an
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Beispielbild laden (1x1 Pixel roter Punkt)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Modifizierte Arbeitsmappe speichern
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo.xlsx");

            // Ausrichtung auf BottomLeft ändern und eine weitere Version speichern
            tileOptions.AlignmentType = RectangleAlignmentType.BottomLeft;
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo_BottomLeft.xlsx");
        }
    }
}
```

### Siehe auch

* enum [RectangleAlignmentType](../../rectanglealignmenttype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


