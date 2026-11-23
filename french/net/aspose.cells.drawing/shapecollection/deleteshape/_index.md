---
title: "ShapeCollection.DeleteShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Supprimer une forme. Si la forme se trouve dans le groupe ou est une forme de commentaire, elle ne sera pas supprimée"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/deleteshape/
---
## ShapeCollection.DeleteShape method

Supprime une forme. Si la forme est dans le groupe ou est une forme de commentaire, elle ne sera pas supprimée.

```csharp
public void DeleteShape(Shape shape)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| forme | Forme |  |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteShapeWithShapeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter la première forme de rectangle
            Shape firstShape = shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Ajouter la deuxième forme de rectangle
            Shape secondShape = shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Supprimer la première forme
            shapes.DeleteShape(firstShape);

            // Enregistrez le classeur
            workbook.Save("DeleteShapeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


