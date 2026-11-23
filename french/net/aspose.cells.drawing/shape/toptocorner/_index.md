---
title: "Shape.TopToCorner"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul en pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shape/toptocorner/
---
## Shape.TopToCorner property

Obtient et définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en pixels.

```csharp
public int TopToCorner { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopToCornerDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangle à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Définir et afficher la propriété TopToCorner
            shape.TopToCorner = 50;
            Console.WriteLine("Shape TopToCorner: " + shape.TopToCorner);

            // Modifier la propriété TopToCorner
            if (shape.TopToCorner == 50)
            {
                shape.TopToCorner = 20;
                Console.WriteLine("Updated Shape TopToCorner: " + shape.TopToCorner);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


