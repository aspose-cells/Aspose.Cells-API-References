---
title: "Shape.GetConnectionPoints"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Obtenez les points de connexion"
type: docs
url: /fr/net/aspose.cells.drawing/shape/getconnectionpoints/
---
## Shape.GetConnectionPoints method

Obtenir les points de connexion

```csharp
public float[][] GetConnectionPoints()
```

### Valeur de retour

[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetConnectionPointsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoute une forme à la feuille de calcul avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Obtenez les points de connexion de la forme
            float[][] points = shape.GetConnectionPoints();

            // Affichez les points de connexion
            Console.WriteLine("Connection Points:");
            for (int i = 0; i < points.Length; i++)
            {
                Console.WriteLine($"Point {i + 1}: X={points[i][0]}, Y={points[i][1]}");
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


