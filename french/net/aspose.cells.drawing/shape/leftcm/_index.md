---
title: "Shape.LeftCM"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente le décalage horizontal de la forme depuis sa colonne de gauche en centimètres"
type: docs
url: /fr/net/aspose.cells.drawing/shape/leftcm/
---
## Shape.LeftCM property

Représente le décalage horizontal de la forme depuis sa colonne de gauche, en unité de centimètres.

```csharp
public double LeftCM { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftCMDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Définir et obtenir la propriété LeftCM
            shape.LeftCM = 3.0;
            Console.WriteLine("Shape left position (cm): " + shape.LeftCM);

            // Modifier la position gauche si elle est de 3 cm
            if (shape.LeftCM == 3.0)
            {
                shape.LeftCM = 1.0;
                Console.WriteLine("Adjusted shape left position (cm): " + shape.LeftCM);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


