---
title: "ThreeDFormat.Perspective"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Liest und setzt den Winkel, aus dem ein ThreeDFormat-Objekt betrachtet werden kann"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/perspective/
---
## ThreeDFormat.Perspective property

Liest und setzt den Winkel, aus dem ein ThreeDFormat-Objekt betrachtet werden kann.

```csharp
public double Perspective { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 200, 100);
            
            // Erhalte das 3D-Format der Form
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Zeige den aktuellen Perspektivwert an
            Console.WriteLine("Current Perspective value: " + threeDFormat.Perspective);

            // Setze neuen Perspektivwert (0 bis 120 Grad)
            threeDFormat.Perspective = 45;
            Console.WriteLine("Perspective set to: " + threeDFormat.Perspective);

            // Wende weitere 3D-Effekte an, um die Perspektivänderung besser zu visualisieren
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Speichere die Arbeitsmappe, um die Auswirkungen zu sehen
            workbook.Save("ThreeDFormatPerspectiveDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


