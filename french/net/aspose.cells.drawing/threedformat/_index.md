---
title: "Classe ThreeDFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.ThreeDFormat. Représente le formatage tridimensionnel d'une forme"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/
---
## ThreeDFormat class

Représente le formatage tridimensionnel d'une forme.

```csharp
public class ThreeDFormat
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BottomBevelHeight](../../aspose.cells.drawing/threedformat/bottombevelheight/) { get; set; } | Obtient et définit la hauteur du biseau inférieur, ou la profondeur d'application dans la forme. En unités de points. |
| [BottomBevelType](../../aspose.cells.drawing/threedformat/bottombeveltype/) { get; set; } | Obtient et définit le type du biseau inférieur, ou la profondeur d'application dans la forme. En unités de points. |
| [BottomBevelWidth](../../aspose.cells.drawing/threedformat/bottombevelwidth/) { get; set; } | Obtient et définit la largeur du biseau inférieur, ou la profondeur d'application dans la forme. En unités de points. |
| [ContourColor](../../aspose.cells.drawing/threedformat/contourcolor/) { get; set; } | Obtient et définit la couleur du contour d'une forme. |
| [ContourWidth](../../aspose.cells.drawing/threedformat/contourwidth/) { get; set; } | Obtient et définit la largeur du contour sur la forme, en unités de points. |
| [ExtrusionColor](../../aspose.cells.drawing/threedformat/extrusioncolor/) { get; set; } | Obtient la couleur d'extrusion d'une forme. |
| [ExtrusionHeight](../../aspose.cells.drawing/threedformat/extrusionheight/) { get; set; } | Obtient et définit la hauteur d'extrusion appliquée à la forme, en unités de points. |
| [LightAngle](../../aspose.cells.drawing/threedformat/lightangle/) { get; set; } | Obtient et définit l'angle des lumières d'extrusion. |
| [Lighting](../../aspose.cells.drawing/threedformat/lighting/) { get; set; } | Obtient et définit le type de dispositif d'éclairage. |
| [LightingDirection](../../aspose.cells.drawing/threedformat/lightingdirection/) { get; set; } | Obtient et définit la direction depuis laquelle le dispositif d'éclairage est orienté par rapport à la scène. |
| [Material](../../aspose.cells.drawing/threedformat/material/) { get; set; } | Représente le matériau prédéfini qui est combiné aux propriétés d'éclairage pour donner l'apparence finale d'une forme. |
| [Perspective](../../aspose.cells.drawing/threedformat/perspective/) { get; set; } | Obtient et définit l'angle sous lequel un objet ThreeDFormat peut être visualisé. |
| [PresetCameraType](../../aspose.cells.drawing/threedformat/presetcameratype/) { get; set; } | Obtient et définit le type de caméra prédéfini pour l'extrusion. |
| [RotationX](../../aspose.cells.drawing/threedformat/rotationx/) { get; set; } | Obtient et définit la rotation de la forme extrudée autour de l'axe x en degrés. |
| [RotationY](../../aspose.cells.drawing/threedformat/rotationy/) { get; set; } | Obtient et définit la rotation de la forme extrudée autour de l'axe y en degrés. |
| [RotationZ](../../aspose.cells.drawing/threedformat/rotationz/) { get; set; } | Obtient et définit la rotation de la forme extrudée autour de l'axe z en degrés. |
| [TopBevelHeight](../../aspose.cells.drawing/threedformat/topbevelheight/) { get; set; } | Obtient et définit la hauteur du biseau supérieur, ou la profondeur d'application dans la forme. En unités de points. |
| [TopBevelType](../../aspose.cells.drawing/threedformat/topbeveltype/) { get; set; } | Obtient et définit le type du biseau supérieur, ou la profondeur d'application dans la forme. En unité de points. |
| [TopBevelWidth](../../aspose.cells.drawing/threedformat/topbevelwidth/) { get; set; } | Obtient et définit la largeur du biseau supérieur, ou la profondeur d'application dans la forme. En unité de points. |
| [Z](../../aspose.cells.drawing/threedformat/z/) { get; set; } | Définit la distance du sol pour la forme 3D. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/threedformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/threedformat/gethashcode/)() | Obtient le hashcode. |

### Exemples

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

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


