---
title: "ThreeDFormat.Z"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Definiert den Abstand vom Boden für die 3D-Form"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/z/
---
## ThreeDFormat.Z property

Definiert den Abstand vom Boden für die 3D-Form.

```csharp
public double Z { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyZDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 100);
            
            // Greife auf das ThreeDFormat der Form zu.
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Aktuellen Z-Wert anzeigen (Abstand vom Boden)
            Console.WriteLine("Current Z value: " + threeDFormat.Z);

            // Neuen Z-Wert setzen, um die Form weiter vom Boden zu entfernen
            threeDFormat.Z = 20;
            Console.WriteLine("New Z value: " + threeDFormat.Z);

            // Weitere 3D-Eigenschaften konfigurieren, um den Effekt sichtbar zu machen
            threeDFormat.ExtrusionHeight = 30;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Arbeitsmappe speichern, um den 3D-Effekt zu sehen
            workbook.Save("ThreeDFormatPropertyZDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


