---
title: "Shape.X"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Shape property. Obtient et définit le décalage horizontal du shape depuis la bordure gauche de la feuille de calcul en pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shape/x/
---
## Shape.X property

Obtient et définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul, en unité de pixels.

```csharp
public int X { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyXDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Définir la position X initiale
            shape.X = 200;
            Console.WriteLine("Initial X position: " + shape.X);

            // Modifier la position X si elle vaut 3 (démonstration de la logique du cas de test)
            if (shape.X == 3)
            {
                shape.X = 1;
            }
            else
            {
                // À des fins de démonstration, changer la position X à 300
                shape.X = 300;
            }

            Console.WriteLine("Final X position: " + shape.X);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


