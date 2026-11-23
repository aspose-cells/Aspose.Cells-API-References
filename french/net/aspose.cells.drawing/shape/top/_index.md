---
title: "Shape.Top"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente le décalage vertical de la forme par rapport à sa ligne supérieure en pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shape/top/
---
## Shape.Top property

Représente le décalage vertical de la forme par rapport à sa ligne supérieure, en pixels.

```csharp
public int Top { get; set; }
```

### Remarques

Si la forme se trouve dans le graphique, représente le décalage vertical de la forme par rapport à sa bordure supérieure.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Définir la position supérieure initiale
            shape.Top = 50;
            Console.WriteLine("Initial Top position: " + shape.Top);

            // Modifier la position supérieure si elle vaut 3 (démontrant la logique du cas de test)
            if (shape.Top == 3)
            {
                shape.Top = 1;
            }
            else
            {
                // À des fins de démonstration, définir à 3 puis appliquer la logique du cas de test
                shape.Top = 3;
                if (shape.Top == 3)
                {
                    shape.Top = 1;
                    Console.WriteLine("Modified Top position: " + shape.Top);
                }
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


