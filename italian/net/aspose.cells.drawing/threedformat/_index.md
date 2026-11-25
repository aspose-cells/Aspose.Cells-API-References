---
title: "Classe ThreeDFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.ThreeDFormat. Rappresenta la formattazione tridimensionale di una forma"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/
---
## ThreeDFormat class

Rappresenta la formattazione tridimensionale di una forma.

```csharp
public class ThreeDFormat
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BottomBevelHeight](../../aspose.cells.drawing/threedformat/bottombevelheight/) { get; set; } | Ottiene e imposta l'altezza del bordo inferiore, o quanto è applicato alla forma. In unità di punti. |
| [BottomBevelType](../../aspose.cells.drawing/threedformat/bottombeveltype/) { get; set; } | Ottiene e imposta il tipo del bordo inferiore, o quanto è applicato alla forma. In unità di punti. |
| [BottomBevelWidth](../../aspose.cells.drawing/threedformat/bottombevelwidth/) { get; set; } | Ottiene e imposta la larghezza del bordo inferiore, o quanto è applicato alla forma. In unità di punti. |
| [ContourColor](../../aspose.cells.drawing/threedformat/contourcolor/) { get; set; } | Ottiene e imposta il colore del contorno su una forma. |
| [ContourWidth](../../aspose.cells.drawing/threedformat/contourwidth/) { get; set; } | Ottiene e imposta la larghezza del contorno sulla forma, in unità di punti. |
| [ExtrusionColor](../../aspose.cells.drawing/threedformat/extrusioncolor/) { get; set; } | Ottiene il colore di estrusione su una forma. |
| [ExtrusionHeight](../../aspose.cells.drawing/threedformat/extrusionheight/) { get; set; } | Ottiene e imposta l'altezza di estrusione applicata alla forma, in unità di punti. |
| [LightAngle](../../aspose.cells.drawing/threedformat/lightangle/) { get; set; } | Ottiene e imposta l'angolo delle luci di estrusione. |
| [Lighting](../../aspose.cells.drawing/threedformat/lighting/) { get; set; } | Ottiene e imposta il tipo di impianto luminoso. |
| [LightingDirection](../../aspose.cells.drawing/threedformat/lightingdirection/) { get; set; } | Ottiene e imposta la direzione da cui l'impianto luminoso è orientato rispetto alla scena. |
| [Material](../../aspose.cells.drawing/threedformat/material/) { get; set; } | Rappresenta il materiale predefinito che viene combinato con le proprietà di illuminazione per fornire l'aspetto finale di una forma. |
| [Perspective](../../aspose.cells.drawing/threedformat/perspective/) { get; set; } | Ottiene e imposta l'angolo da cui un oggetto ThreeDFormat può essere visualizzato. |
| [PresetCameraType](../../aspose.cells.drawing/threedformat/presetcameratype/) { get; set; } | Ottiene e imposta il tipo di telecamera predefinita per l'estrusione. |
| [RotationX](../../aspose.cells.drawing/threedformat/rotationx/) { get; set; } | Ottiene e imposta la rotazione della forma estrusa attorno all'asse x in gradi. |
| [RotationY](../../aspose.cells.drawing/threedformat/rotationy/) { get; set; } | Ottiene e imposta la rotazione della forma estrusa attorno all'asse y in gradi. |
| [RotationZ](../../aspose.cells.drawing/threedformat/rotationz/) { get; set; } | Ottiene e imposta la rotazione della forma estrusa attorno all'asse z in gradi. |
| [TopBevelHeight](../../aspose.cells.drawing/threedformat/topbevelheight/) { get; set; } | Ottiene e imposta l'altezza del bordo superiore, o quanto è applicato alla forma. In unità di punti. |
| [TopBevelType](../../aspose.cells.drawing/threedformat/topbeveltype/) { get; set; } | Ottiene e imposta il tipo del bordo superiore, o quanto profondamente viene applicato nella forma. In unità di punti. |
| [TopBevelWidth](../../aspose.cells.drawing/threedformat/topbevelwidth/) { get; set; } | Ottiene e imposta la larghezza del bordo superiore, o quanto profondamente viene applicato nella forma. In unità di punti. |
| [Z](../../aspose.cells.drawing/threedformat/z/) { get; set; } | Definisce la distanza dal suolo per la forma 3D. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/threedformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/threedformat/gethashcode/)() | Ottiene il codice hash. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


