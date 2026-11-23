---
title: "CustomGeometry.Paths"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CustomGeometry. Obtient les informations de la collection de chemins lorsque la forme est une autoshape NotPrimitive"
type: docs
url: /fr/net/aspose.cells.drawing/customgeometry/paths/
---
## CustomGeometry.Paths property

Obtient les informations de la collection de chemins lorsque la forme est une autoshape NotPrimitive

```csharp
public ShapePathCollection Paths { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CustomGeometryPropertyPathsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme personnalisée avec une géométrie non primitive (paramètres fixes)
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 10, 10, 400, 400);
            
            // Accéder à la géométrie personnalisée via un transtypage explicite
            CustomGeometry geometry = (CustomGeometry)shape.Geometry;
            
            // Obtenir la collection de chemins
            ShapePathCollection paths = geometry.Paths;
            Console.WriteLine($"Initial path count: {paths.Count}");

            // Créer un nouveau chemin de forme en utilisant des commandes de dessin
            paths.Add(); // Creates a new path in the collection
            ShapePath newPath = paths[paths.Count - 1];
            newPath.MoveTo(0, 0);
            newPath.LineTo(10000, 0);
            newPath.LineTo(10000, 10000);
            newPath.LineTo(0, 10000);
            newPath.Close();

            // Aucun ajout explicite nécessaire puisque le chemin a été créé dans la collection
            Console.WriteLine($"New path count after modification: {paths.Count}");

            // Enregistrer pour démontrer les modifications persistantes
            workbook.Save("CustomGeometryPathsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapePathCollection](../../shapepathcollection/)
* class [CustomGeometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


