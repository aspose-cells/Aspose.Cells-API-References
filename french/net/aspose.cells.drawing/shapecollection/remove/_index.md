---
title: "ShapeCollection.Remove"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Supprime la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

Supprime la forme.

```csharp
public void Remove(Shape shape)
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
    public class ShapeCollectionMethodRemoveWithShapeDemo
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

            // Obtenir la première forme par nom ou indice
            Shape shapeToRemove = shapes["Rectangle 1"]; // or shapes[0];
            
            if (shapeToRemove != null)
            {
                // Supprimer la forme de la collection
                shapes.Remove(shapeToRemove);
            }

            // Enregistrez le classeur
            workbook.Save("ShapeRemoveDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


