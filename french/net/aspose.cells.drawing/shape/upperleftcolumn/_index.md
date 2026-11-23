---
title: "Shape.UpperLeftColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente l'indice de colonne du coin supérieur gauche"
type: docs
url: /fr/net/aspose.cells.drawing/shape/upperleftcolumn/
---
## Shape.UpperLeftColumn property

Représente l'index de la colonne du coin supérieur gauche.

```csharp
public int UpperLeftColumn { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoute une forme à la feuille de calcul avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 100);

            // Définir et démontrer la propriété UpperLeftColumn
            shape.UpperLeftColumn = 3;
            Console.WriteLine("Shape's initial leftColumn: " + shape.UpperLeftColumn);

            // Modifier l'UpperLeftColumn
            if (shape.UpperLeftColumn == 3)
            {
                shape.UpperLeftColumn = 1;
                Console.WriteLine("Shape's modified leftColumn: " + shape.UpperLeftColumn);
            }

            // Enregistrez le classeur
            workbook.Save("ShapeUpperLeftColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


