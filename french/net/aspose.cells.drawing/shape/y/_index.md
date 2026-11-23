---
title: "Shape.Y"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille, en unités de pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shape/y/
---
## Shape.Y property

Obtient et définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en pixels.

```csharp
public int Y { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyYDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Définir et démontrer la propriété Y
            shape.Y = 200;
            Console.WriteLine("Shape Y position: " + shape.Y);

            // Modifier la position Y en fonction d'une condition
            if (shape.Y == 200)
                shape.Y = 100;

            Console.WriteLine("Updated Shape Y position: " + shape.Y);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


