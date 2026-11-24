---
title: "ThreeDFormat.LightAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Liest und setzt den Winkel der Extrusionslichter"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/lightangle/
---
## ThreeDFormat.LightAngle property

Liest und setzt den Winkel der Extrusionslichter.

```csharp
public double LightAngle { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightAngleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D Format Demo";
            
            // Greife auf das ThreeDFormat der Form zu.
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Zeige den aktuellen LightAngle-Wert an
            Console.WriteLine("Current LightAngle value: " + threeDFormat.LightAngle);

            // Setze neuen LightAngle-Wert (0 bis 359,9 Grad)
            threeDFormat.LightAngle = 45;
            Console.WriteLine("New LightAngle value: " + threeDFormat.LightAngle);

            // Konfiguriere weitere 3D-Eigenschaften, um die Wirkung von LightAngle zu sehen
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Speichere die Arbeitsmappe, um die Auswirkungen zu sehen
            workbook.Save("ThreeDFormatLightAngleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


