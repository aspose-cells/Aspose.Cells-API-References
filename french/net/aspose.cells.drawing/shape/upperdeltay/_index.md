---
title: "Shape.UpperDeltaY"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient ou définit le décalage vertical de la forme depuis sa ligne du coin supérieur gauche."
type: docs
url: /fr/net/aspose.cells.drawing/shape/upperdeltay/
---
## Shape.UpperDeltaY property

Obtient ou définit le décalage vertical de la forme depuis la ligne de son coin supérieur gauche.

```csharp
public int UpperDeltaY { get; set; }
```

### Remarques

La plage de valeurs est de 0 à 256.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer la propriété UpperDeltaY
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Définir et afficher la valeur initiale de UpperDeltaY
            shape.UpperDeltaY = 3;
            Console.WriteLine("Initial UpperDeltaY: " + shape.UpperDeltaY);

            // Modifier la valeur de UpperDeltaY
            if (shape.UpperDeltaY == 3)
            {
                shape.UpperDeltaY = 1;
                Console.WriteLine("Modified UpperDeltaY: " + shape.UpperDeltaY);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


