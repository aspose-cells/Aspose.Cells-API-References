---
title: "ShapePathCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapePathCollection. Obtient un chemin de création"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathcollection/item/
---
## ShapePathCollection indexer

Obtient un chemin de création.

```csharp
public ShapePath this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

Renvoie l'objet [`ShapePath`](../../shapepath/).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme personnalisée (forme non primitive) avec les paramètres corrects
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 10, 10, 200, 200, 0, 0);

            // Accédez à la ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // Ajouter un nouveau chemin
            int pathIndex = shapePaths.Add();

            // Accéder au chemin en utilisant la propriété Item
            ShapePath newPath = shapePaths[pathIndex];

            // Informations de sortie
            Console.WriteLine("Path count: " + shapePaths.Count);
            Console.WriteLine("Path segment count: " + newPath.PathSegementList.Count);

            // Enregistrez le classeur
            workbook.Save("ShapePathCollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapePath](../../shapepath/)
* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


