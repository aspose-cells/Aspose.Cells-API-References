---
title: "ThreeDFormat.RotationX"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Liest und schreibt die Drehung der extrudierten Form um die X-Achse in Grad"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/rotationx/
---
## ThreeDFormat.RotationX property

Liest und setzt die Drehung der extrudierten Form um die X-Achse in Grad.

```csharp
public double RotationX { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationXDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 2, 2, 200, 100, 100);
            
            // 3D-Format abrufen (es ist nicht nötig, 3D-Effekte zu \"aktivieren\" – einfach die Eigenschaften setzen)
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Aktuellen RotationX-Wert anzeigen
            Console.WriteLine("Current RotationX value: " + threeDFormat.RotationX);

            // Neuen RotationX-Wert setzen (Drehung um die X-Achse in Grad)
            threeDFormat.RotationX = 45;
            Console.WriteLine("New RotationX value: " + threeDFormat.RotationX);

            // Weitere 3D-Eigenschaften setzen, um die Drehung sichtbar zu machen
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Speichere die Arbeitsmappe, um die Auswirkungen zu sehen
            workbook.Save("ThreeDFormatRotationXDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


