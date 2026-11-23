---
title: "ShapeCollection.Group"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Regroupe les formes"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/group/
---
## ShapeCollection.Group method

Regrouper les formes.

```csharp
public GroupShape Group(Shape[] groupItems)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| groupItems | Shape[] | les éléments du groupe. |

### Valeur de retour

Renvoie la forme du groupe.

### Remarques

La forme dans groupItems ne doit pas être groupée. La forme doit se trouver dans cette collection Shapes.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodGroupWithShapeArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter la première forme de rectangle
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Ajouter la deuxième forme de rectangle
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Créer un tableau avec les formes à regrouper
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Grouper les formes
            GroupShape groupShape = shapes.Group(shapesArr);

            // Enregistrez le classeur
            workbook.Save("GroupShapesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GroupShape](../../groupshape/)
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


