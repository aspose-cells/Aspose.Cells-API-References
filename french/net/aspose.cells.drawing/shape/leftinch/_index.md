---
title: "Shape.LeftInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente le décalage horizontal de la forme par rapport à sa colonne de gauche en unité de pouces"
type: docs
url: /fr/net/aspose.cells.drawing/shape/leftinch/
---
## Shape.LeftInch property

Représente le décalage horizontal de la forme depuis sa colonne de gauche, en unité de pouces.

```csharp
public double LeftInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Définir et démontrer la propriété LeftInch
            shape.LeftInch = 3;
            Console.WriteLine("Shape left position (inches): " + shape.LeftInch);

            // Modifier la position gauche si elle est de 3 pouces
            if (shape.LeftInch == 3)
            {
                shape.LeftInch = 1;
                Console.WriteLine("Adjusted shape left position (inches): " + shape.LeftInch);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


