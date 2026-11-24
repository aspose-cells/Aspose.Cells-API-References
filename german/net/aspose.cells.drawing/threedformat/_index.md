---
title: "Klasse ThreeDFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ThreeDFormat-Klasse. Stellt die dreidimensionale Formatierung einer Form dar"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/
---
## ThreeDFormat class

Stellt die dreidimensionale Formatierung einer Form dar.

```csharp
public class ThreeDFormat
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BottomBevelHeight](../../aspose.cells.drawing/threedformat/bottombevelheight/) { get; set; } | Liest und setzt die Höhe der unteren Abschrägung bzw. wie weit sie in die Form angewendet wird. In Punkten. |
| [BottomBevelType](../../aspose.cells.drawing/threedformat/bottombeveltype/) { get; set; } | Liest und setzt den Typ der unteren Abschrägung bzw. wie weit sie in die Form angewendet wird. In Punkten. |
| [BottomBevelWidth](../../aspose.cells.drawing/threedformat/bottombevelwidth/) { get; set; } | Liest und setzt die Breite der unteren Abschrägung bzw. wie weit sie in die Form angewendet wird. In Punkten. |
| [ContourColor](../../aspose.cells.drawing/threedformat/contourcolor/) { get; set; } | Liest und setzt die Konturfarbe einer Form. |
| [ContourWidth](../../aspose.cells.drawing/threedformat/contourwidth/) { get; set; } | Liest und setzt die Konturbreite der Form, in Punkten. |
| [ExtrusionColor](../../aspose.cells.drawing/threedformat/extrusioncolor/) { get; set; } | Liest die Extrusionsfarbe einer Form. |
| [ExtrusionHeight](../../aspose.cells.drawing/threedformat/extrusionheight/) { get; set; } | Liest und setzt die Extrusionshöhe, die auf die Form angewendet wird, in Punkten. |
| [LightAngle](../../aspose.cells.drawing/threedformat/lightangle/) { get; set; } | Liest und setzt den Winkel der Extrusionslichter. |
| [Lighting](../../aspose.cells.drawing/threedformat/lighting/) { get; set; } | Liest und setzt den Typ des Lichtgestells. |
| [LightingDirection](../../aspose.cells.drawing/threedformat/lightingdirection/) { get; set; } | Liest und setzt die Richtung, aus der das Lichtgestell relativ zur Szene ausgerichtet ist. |
| [Material](../../aspose.cells.drawing/threedformat/material/) { get; set; } | Stellt das voreingestellte Material dar, das mit den Lichteigenschaften kombiniert wird, um das endgültige Aussehen einer Form zu erzeugen. |
| [Perspective](../../aspose.cells.drawing/threedformat/perspective/) { get; set; } | Liest und setzt den Winkel, aus dem ein ThreeDFormat-Objekt betrachtet werden kann. |
| [PresetCameraType](../../aspose.cells.drawing/threedformat/presetcameratype/) { get; set; } | Liest und setzt den voreingestellten Kameratyp für die Extrusion. |
| [RotationX](../../aspose.cells.drawing/threedformat/rotationx/) { get; set; } | Liest und setzt die Drehung der extrudierten Form um die X-Achse in Grad. |
| [RotationY](../../aspose.cells.drawing/threedformat/rotationy/) { get; set; } | Liest und setzt die Drehung der extrudierten Form um die Y-Achse in Grad. |
| [RotationZ](../../aspose.cells.drawing/threedformat/rotationz/) { get; set; } | Liest und setzt die Drehung der extrudierten Form um die Z-Achse in Grad. |
| [TopBevelHeight](../../aspose.cells.drawing/threedformat/topbevelheight/) { get; set; } | Liest und setzt die Höhe der oberen Abschrägung bzw. wie tief sie in die Form eingreift. In Punkten. |
| [TopBevelType](../../aspose.cells.drawing/threedformat/topbeveltype/) { get; set; } | Liest und setzt den Typ der oberen Abschrägung bzw. wie tief sie in die Form eingreift. In Punkten. |
| [TopBevelWidth](../../aspose.cells.drawing/threedformat/topbevelwidth/) { get; set; } | Liest und setzt die Breite der oberen Abschrägung bzw. wie tief sie in die Form eingreift. In Punkten. |
| [Z](../../aspose.cells.drawing/threedformat/z/) { get; set; } | Definiert den Abstand vom Boden für die 3D-Form. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/threedformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/threedformat/gethashcode/)() | Liest den Hashcode. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassThreeDFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 210, 210, 200, 200);
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.ExtrusionHeight = 20;

            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


