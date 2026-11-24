---
title: "ThreeDFormat.RotationZ"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Liest und schreibt die Drehung der extrudierten Form um die Z-Achse in Grad"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/rotationz/
---
## ThreeDFormat.RotationZ property

Liest und setzt die Drehung der extrudierten Form um die Z-Achse in Grad.

```csharp
public double RotationZ { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationZDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 0, 100, 150);
            shape.Text = "3D Rotation Demo";
            
            // Greife auf das ThreeDFormat der Form zu.
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Aktuellen RotationZ-Wert anzeigen
            Console.WriteLine("Current RotationZ value: " + threeDFormat.RotationZ);

            // Neue RotationZ-Werte setzen und Effekte demonstrieren
            threeDFormat.RotationZ = 45;
            Console.WriteLine("Shape rotated 45 degrees around Z-axis");

            // Weitere 3D-Eigenschaften anwenden, um die Drehung sichtbar zu machen
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Arbeitsmappe mit den 3D-Effekten speichern
            workbook.Save("ThreeDFormatRotationZDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


