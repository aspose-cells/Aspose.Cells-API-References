---
title: "ShapeCollection.Ungroup"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Dégroupe les éléments de forme"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/ungroup/
---
## ShapeCollection.Ungroup method

Dégroupe les éléments de forme.

```csharp
public void Ungroup(GroupShape group)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| groupe | GroupShape | La forme de groupe. |

### Remarques

Si la forme de groupe est groupée par une autre forme de groupe, rien ne sera fait.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUngroupWithGroupShapeDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter la première forme de rectangle
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Ajouter la deuxième forme de rectangle
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Créer un tableau de formes à grouper
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Grouper les formes
            GroupShape groupShape = shapes.Group(shapesArr);

            // Dégrouper la forme de groupe
            shapes.Ungroup(groupShape);
        }
    }
}
```

### Voir aussi

* class [GroupShape](../../groupshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


