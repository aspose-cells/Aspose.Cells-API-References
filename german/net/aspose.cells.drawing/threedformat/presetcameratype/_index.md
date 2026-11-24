---
title: "ThreeDFormat.PresetCameraType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Liest und schreibt den voreingestellten Kameratyp für die Extrusion"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/presetcameratype/
---
## ThreeDFormat.PresetCameraType property

Liest und setzt den voreingestellten Kameratyp für die Extrusion.

```csharp
public PresetCameraType PresetCameraType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPresetCameraTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 200);
            
            // Hole das ThreeDFormat der Form.
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Aktuellen PresetCameraType-Wert anzeigen
            Console.WriteLine("Current PresetCameraType: " + threeDFormat.PresetCameraType);

            // Neuen PresetCameraType-Wert setzen
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveHeroicLeftFacing;

            // Zusätzliche 3D-Formatierung anwenden, um den Effekt sichtbar zu machen
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Neuen PresetCameraType-Wert anzeigen
            Console.WriteLine("New PresetCameraType: " + threeDFormat.PresetCameraType);

            // Arbeitsmappe speichern, um den Effekt zu zeigen
            workbook.Save("ThreeDFormatPresetCameraTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PresetCameraType](../../presetcameratype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


