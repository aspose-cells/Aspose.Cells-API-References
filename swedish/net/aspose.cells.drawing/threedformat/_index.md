---
title: "Klass ThreeDFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ThreeDFormat-klass. Representerar en forms tredimensionella formatering"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/
---
## ThreeDFormat class

Representerar en forms tredimensionella formatering.

```csharp
public class ThreeDFormat
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BottomBevelHeight](../../aspose.cells.drawing/threedformat/bottombevelheight/) { get; set; } | Hämtar och anger höjden på den nedre fasen, eller hur långt in i formen den tillämpas. I enheten Points. |
| [BottomBevelType](../../aspose.cells.drawing/threedformat/bottombeveltype/) { get; set; } | Hämtar och anger typen av den nedre fasen, eller hur långt in i formen den tillämpas. I enheten Points. |
| [BottomBevelWidth](../../aspose.cells.drawing/threedformat/bottombevelwidth/) { get; set; } | Hämtar och anger bredden på den nedre fasen, eller hur långt in i formen den tillämpas. I enheten Points. |
| [ContourColor](../../aspose.cells.drawing/threedformat/contourcolor/) { get; set; } | Hämtar och anger konturfärgen på en form. |
| [ContourWidth](../../aspose.cells.drawing/threedformat/contourwidth/) { get; set; } | Hämtar och anger konturbredden på formen, i enheten punkter. |
| [ExtrusionColor](../../aspose.cells.drawing/threedformat/extrusioncolor/) { get; set; } | Hämtar extruderingsfärgen på en form. |
| [ExtrusionHeight](../../aspose.cells.drawing/threedformat/extrusionheight/) { get; set; } | Hämtar och anger extruderingshöjden som tillämpas på formen, i enheten punkter. |
| [LightAngle](../../aspose.cells.drawing/threedformat/lightangle/) { get; set; } | Hämtar och anger vinkeln på extruderingsljusen. |
| [Lighting](../../aspose.cells.drawing/threedformat/lighting/) { get; set; } | Hämtar och anger typen av ljusanordning. |
| [LightingDirection](../../aspose.cells.drawing/threedformat/lightingdirection/) { get; set; } | Hämtar och anger riktningen från vilken ljusanordningen är orienterad i förhållande till scenen. |
| [Material](../../aspose.cells.drawing/threedformat/material/) { get; set; } | Representerar det förinställda materialet som kombineras med ljusegenskaperna för att ge den slutgiltiga utseendet och känslan av en form. |
| [Perspective](../../aspose.cells.drawing/threedformat/perspective/) { get; set; } | Hämtar och anger vinkeln vid vilken ett ThreeDFormat-objekt kan visas. |
| [PresetCameraType](../../aspose.cells.drawing/threedformat/presetcameratype/) { get; set; } | Hämtar och anger den förinställda kameratypen för extrusion. |
| [RotationX](../../aspose.cells.drawing/threedformat/rotationx/) { get; set; } | Hämtar och anger rotationen av den extruderade formen runt x-axeln i grader. |
| [RotationY](../../aspose.cells.drawing/threedformat/rotationy/) { get; set; } | Hämtar och anger rotationen av den extruderade formen runt y-axeln i grader. |
| [RotationZ](../../aspose.cells.drawing/threedformat/rotationz/) { get; set; } | Hämtar och anger rotationen av den extruderade formen runt z-axeln i grader. |
| [TopBevelHeight](../../aspose.cells.drawing/threedformat/topbevelheight/) { get; set; } | Hämtar och anger höjden på den övre fasen, eller hur långt in i formen den appliceras. I enheten punkter. |
| [TopBevelType](../../aspose.cells.drawing/threedformat/topbeveltype/) { get; set; } | Hämtar och anger typen av den övre fasen, eller hur långt in i formen den appliceras. I enheten punkter. |
| [TopBevelWidth](../../aspose.cells.drawing/threedformat/topbevelwidth/) { get; set; } | Hämtar och anger bredden på den övre fasen, eller hur långt in i formen den appliceras. I enheten punkter. |
| [Z](../../aspose.cells.drawing/threedformat/z/) { get; set; } | Definierar avståndet från marken för den 3D-formen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/threedformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/threedformat/gethashcode/)() | Hämtar hashkod. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


