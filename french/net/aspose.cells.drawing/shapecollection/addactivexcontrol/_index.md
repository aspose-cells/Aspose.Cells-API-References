---
title: "ShapeCollection.AddActiveXControl"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Crée un contrôle Activex"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addactivexcontrol/
---
## ShapeCollection.AddActiveXControl method

Crée un contrôle Activex.

```csharp
public Shape AddActiveXControl(ControlType type, int topRow, int top, int leftColumn, int left, 
    int width, int height)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ControlType | Le type du contrôle. |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de Shape par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de Shape par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur de Shape, en unité de pixel. |
| largeur | Int32 | Représente la largeur de Shape, en unité de pixel. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddActiveXControlWithControlTypeInt32Int32Int32Int3Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape activeXControl = shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 
                1,  // upperLeftRow
                0,  // top
                1,  // upperLeftColumn
                0,  // left
                100,  // width
                50   // height
            );

            workbook.Save("AddActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* enum [ControlType](../../../aspose.cells.drawing.activexcontrols/controltype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


