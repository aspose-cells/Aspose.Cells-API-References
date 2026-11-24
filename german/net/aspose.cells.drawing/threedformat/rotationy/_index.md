---
title: "ThreeDFormat.RotationY"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Gibt die Drehung der extrudierten Form um die Y-Achse in Grad zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.drawing/threedformat/rotationy/
---
## ThreeDFormat.RotationY property

Liest und setzt die Drehung der extrudierten Form um die Y-Achse in Grad.

```csharp
public double RotationY { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationYDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 100, 150, 150);
            shape.Text = "3D Rotation Demo";
            
            // Greife auf das ThreeDFormat der Form zu.
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Aktuellen RotationY-Wert anzeigen.
            Console.WriteLine("Current RotationY value: " + threeDFormat.RotationY);

            // Setze neue RotationY-Werte und zeige die Effekte.
            threeDFormat.RotationY = 15;
            Console.WriteLine("Shape rotated 15 degrees around Y-axis");

            // Wende weitere 3D-Eigenschaften an, um den Effekt sichtbar zu machen.
            threeDFormat.ExtrusionHeight = 5;
            threeDFormat.ContourWidth = 1;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Speichere die Arbeitsmappe, um die Effekte zu zeigen.
            workbook.Save("ThreeDFormatRotationYDemo.xlsx");

            // Drehe erneut und speichere eine weitere Version.
            threeDFormat.RotationY = 45;
            workbook.Save("ThreeDFormatRotationYDemo_45degrees.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


