---
title: "ThreeDFormat.LightingDirection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat property. Gibt die Richtung zurück, aus der das Lichtgestell relativ zur Szene ausgerichtet ist, und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/lightingdirection/
---
## ThreeDFormat.LightingDirection property

Liest und setzt die Richtung, aus der das Lichtgestell relativ zur Szene ausgerichtet ist.

```csharp
public LightRigDirectionType LightingDirection { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDirectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D Lighting Direction Demo";
            
            // Hole das ThreeDFormat der Form.
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Initiale 3D‑Eigenschaften festlegen
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.Material = PresetMaterialType.Plastic;

            // Aktuelle Beleuchtungsrichtung anzeigen
            Console.WriteLine("Current LightingDirection: " + threeDFormat.LightingDirection);

            // Beleuchtungsrichtung ändern und die Effekte beobachten
            threeDFormat.LightingDirection = LightRigDirectionType.TopLeft;
            Console.WriteLine("Changed LightingDirection to TopLeft");

            // Zu einer anderen Richtung wechseln
            threeDFormat.LightingDirection = LightRigDirectionType.BottomRight;
            Console.WriteLine("Changed LightingDirection to BottomRight");

            // Arbeitsmappe speichern, um die visuellen Effekte zu sehen
            workbook.Save("ThreeDFormatLightingDirectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LightRigDirectionType](../../lightrigdirectiontype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


