---
title: "ThreeDFormat.Lighting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat property. Gibt den Typ des Lichtgestells zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/lighting/
---
## ThreeDFormat.Lighting property

Liest und setzt den Typ des Lichtgestells.

```csharp
public LightRigType Lighting { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 200);
            shape.Text = "3D Lighting Demo";
            
            // Hole das ThreeDFormat der Form.
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Aktuellen Beleuchtungswert anzeigen
            Console.WriteLine("Current Lighting value: " + threeDFormat.Lighting);

            // Verschiedene Beleuchtungstypen festlegen und die Effekte beobachten
            threeDFormat.Lighting = LightRigType.BrightRoom;
            Console.WriteLine("Changed to BrightRoom lighting");

            // Weitere 3D‑Eigenschaften anwenden, um den Lichteffekt besser zu sehen
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;

            // Mit dem ersten Beleuchtungstyp speichern
            workbook.Save("BrightRoomLighting.xlsx");

            // Zu einem anderen Beleuchtungstyp wechseln
            threeDFormat.Lighting = LightRigType.Sunset;
            Console.WriteLine("Changed to Sunset lighting");
            workbook.Save("SunsetLighting.xlsx");

            // Zu einem dritten Beleuchtungstyp wechseln
            threeDFormat.Lighting = LightRigType.ThreePoint;
            Console.WriteLine("Changed to ThreePoint lighting");
            workbook.Save("ThreePointLighting.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LightRigType](../../lightrigtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


