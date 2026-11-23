---
title: "Shape.Paths"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient les chemins d'une forme géométrique personnalisée"
type: docs
url: /fr/net/aspose.cells.drawing/shape/paths/
---
## Shape.Paths property

Obtient les chemins d'une forme géométrique personnalisée.

```csharp
public ShapePathCollection Paths { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPathsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme personnalisée (rectangle) avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 1, 1, 100, 150);

            // Vérifiez si la forme possède des chemins de géométrie personnalisés
            if (shape.Paths != null)
            {
                Console.WriteLine("Shape has custom geometry paths:");
                Console.WriteLine($"Number of paths: {shape.Paths.Count}");
                
                // Ajoutez un nouveau chemin à la géométrie de la forme
                int newPathIndex = shape.Paths.Add();
                Console.WriteLine($"Added new path at index: {newPathIndex}");
            }
            else
            {
                Console.WriteLine("No custom geometry path.");
            }
        }
    }
}
```

### Voir aussi

* class [ShapePathCollection](../../shapepathcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


