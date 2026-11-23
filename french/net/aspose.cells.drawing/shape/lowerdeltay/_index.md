---
title: "Shape.LowerDeltaY"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient ou définit le décalage vertical de la forme à partir de la ligne de son coin inférieur droit"
type: docs
url: /fr/net/aspose.cells.drawing/shape/lowerdeltay/
---
## Shape.LowerDeltaY property

Obtient ou définit le décalage vertical de la forme par rapport à la ligne de son coin inférieur droit.

```csharp
public int LowerDeltaY { get; set; }
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
    public class ShapePropertyLowerDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Définir et démontrer la propriété LowerDeltaY
            shape.LowerDeltaY = 20;
            Console.WriteLine("Initial LowerDeltaY: " + shape.LowerDeltaY);

            // Modifier LowerDeltaY de manière conditionnelle
            if (shape.LowerDeltaY == 20)
            {
                shape.LowerDeltaY = 10;
                Console.WriteLine("Modified LowerDeltaY: " + shape.LowerDeltaY);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


