---
title: "Shape.UpperLeftRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente l'index de la ligne supérieure"
type: docs
url: /fr/net/aspose.cells.drawing/shape/upperleftrow/
---
## Shape.UpperLeftRow property

Représente l'index de la ligne supérieure.

```csharp
public int UpperLeftRow { get; set; }
```

### Remarques

Si la forme est dans la forme ou dans le groupe, UpperLeftRow sera ignoré.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Définir et démontrer la propriété UpperLeftRow
            shape.UpperLeftRow = 3;
            Console.WriteLine("Shape's initial topRow: " + shape.UpperLeftRow);

            // Modifier UpperLeftRow en fonction de la condition
            if (shape.UpperLeftRow == 3)
                shape.UpperLeftRow = 1;

            Console.WriteLine("Shape's modified topRow: " + shape.UpperLeftRow);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


