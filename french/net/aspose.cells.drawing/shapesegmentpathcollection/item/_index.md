---
title: "ShapeSegmentPathCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeSegmentPathCollection. Obtient l'objet ShapeSegmentPath"
type: docs
url: /fr/net/aspose.cells.drawing/shapesegmentpathcollection/item/
---
## ShapeSegmentPathCollection indexer

Obtient l'objet [`ShapeSegmentPath`](../../shapesegmentpath/).

```csharp
public ShapeSegmentPath this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

Renvoie un objet [`ShapeSegmentPath`](../../shapesegmentpath/).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Démarrer un nouveau chemin
            path.MoveTo(10, 10);

            // Dessine un segment de ligne
            path.LineTo(100, 100);

            // Accéder à la propriété PathSegementList
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;


            segmentPaths.Add(ShapePathType.Close);

            // Afficher le nombre de segments de chemin
            Console.WriteLine("Number of path segments: " + segmentPaths.Count);
          
            
            // Démontrer la lecture de la propriété Item
            for (int i = 0; i < segmentPaths.Count; i++)
            {
                ShapeSegmentPath segment = segmentPaths[i];
                Console.WriteLine($"Segment {i} type: {segment.Type}");
            }

            //ajouter une forme libre
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
            // Enregistrez le classeur
            workbook.Save("ShapeSegmentPathCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeSegmentPath](../../shapesegmentpath/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


