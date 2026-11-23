---
title: "ShapeSegmentPathCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeSegmentPathCollection. Ajouter un segment de chemin dans le chemin de création"
type: docs
url: /fr/net/aspose.cells.drawing/shapesegmentpathcollection/add/
---
## ShapeSegmentPathCollection.Add method

Ajoute un chemin de segment dans le chemin de création.

```csharp
public int Add(ShapePathType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ShapePathType | Le type de chemin. |

### Valeur de retour

Renvoie la position de l'objet [`ShapeSegmentPath`](../../shapesegmentpath/) dans la liste.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionMethodAddWithShapePathTypeDemo
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
            ShapeSegmentPathCollection segmentList = path.PathSegementList;

            segmentList.Add(ShapePathType.Close);

            // Afficher le nombre de segments de chemin
            Console.WriteLine("Number of path segments: " + segmentList.Count);

            // Itérer à travers chaque segment et afficher son type
            foreach (ShapeSegmentPath segment in segmentList)
            {
                Console.WriteLine("Segment type: " + segment.Type);
            }

           
            //ajouter une forme libre
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Enregistrez le classeur pour observer les modifications de forme
            workbook.Save("ShapeSegmentPathCollectionAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


