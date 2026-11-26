---
title: "Clase ThreeDFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ThreeDFormat. Representa el formato tridimensional de una forma"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/
---
## ThreeDFormat class

Representa el formato tridimensional de una forma.

```csharp
public class ThreeDFormat
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BottomBevelHeight](../../aspose.cells.drawing/threedformat/bottombevelheight/) { get; set; } | Obtiene y establece la altura del bisel inferior, o cuán profundo se aplica en la forma. En unidades de puntos. |
| [BottomBevelType](../../aspose.cells.drawing/threedformat/bottombeveltype/) { get; set; } | Obtiene y establece el tipo del bisel inferior, o cuán profundo se aplica en la forma. En unidades de puntos. |
| [BottomBevelWidth](../../aspose.cells.drawing/threedformat/bottombevelwidth/) { get; set; } | Obtiene y establece el ancho del bisel inferior, o cuán profundo se aplica en la forma. En unidades de puntos. |
| [ContourColor](../../aspose.cells.drawing/threedformat/contourcolor/) { get; set; } | Obtiene y establece el color del contorno en una forma. |
| [ContourWidth](../../aspose.cells.drawing/threedformat/contourwidth/) { get; set; } | Obtiene y establece el ancho del contorno en la forma, en unidades de puntos. |
| [ExtrusionColor](../../aspose.cells.drawing/threedformat/extrusioncolor/) { get; set; } | Obtiene el color de extrusión en una forma. |
| [ExtrusionHeight](../../aspose.cells.drawing/threedformat/extrusionheight/) { get; set; } | Obtiene y establece la altura de extrusión aplicada a la forma, en unidades de puntos. |
| [LightAngle](../../aspose.cells.drawing/threedformat/lightangle/) { get; set; } | Obtiene y establece el ángulo de las luces de extrusión. |
| [Lighting](../../aspose.cells.drawing/threedformat/lighting/) { get; set; } | Obtiene y establece el tipo de configuración de luz. |
| [LightingDirection](../../aspose.cells.drawing/threedformat/lightingdirection/) { get; set; } | Obtiene y establece la dirección desde la cual se orienta la configuración de luz en relación con la escena. |
| [Material](../../aspose.cells.drawing/threedformat/material/) { get; set; } | Representa el material preestablecido que se combina con las propiedades de iluminación para dar el aspecto y la sensación final de una forma. |
| [Perspective](../../aspose.cells.drawing/threedformat/perspective/) { get; set; } | Obtiene y establece el ángulo desde el cual se puede ver un objeto ThreeDFormat. |
| [PresetCameraType](../../aspose.cells.drawing/threedformat/presetcameratype/) { get; set; } | Obtiene y establece el tipo de cámara preestablecida de extrusión. |
| [RotationX](../../aspose.cells.drawing/threedformat/rotationx/) { get; set; } | Obtiene y establece la rotación de la forma extruida alrededor del eje x en grados. |
| [RotationY](../../aspose.cells.drawing/threedformat/rotationy/) { get; set; } | Obtiene y establece la rotación de la forma extruida alrededor del eje y en grados. |
| [RotationZ](../../aspose.cells.drawing/threedformat/rotationz/) { get; set; } | Obtiene y establece la rotación de la forma extruida alrededor del eje z en grados. |
| [TopBevelHeight](../../aspose.cells.drawing/threedformat/topbevelheight/) { get; set; } | Obtiene y establece la altura del bisel superior, o cuán profundo se aplica en la forma. En unidades de puntos. |
| [TopBevelType](../../aspose.cells.drawing/threedformat/topbeveltype/) { get; set; } | Obtiene y establece el tipo del bisel superior, o cuán profundo se aplica en la forma. En unidades de puntos. |
| [TopBevelWidth](../../aspose.cells.drawing/threedformat/topbevelwidth/) { get; set; } | Obtiene y establece el ancho del bisel superior, o cuán profundo se aplica en la forma. En unidades de puntos. |
| [Z](../../aspose.cells.drawing/threedformat/z/) { get; set; } | Define la distancia desde el suelo para la forma 3D. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/threedformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/threedformat/gethashcode/)() | Obtiene el código hash. |

### Ejemplos

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

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


