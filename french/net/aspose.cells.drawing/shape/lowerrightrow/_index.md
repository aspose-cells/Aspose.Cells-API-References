---
title: "Shape.LowerRightRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente l'indice de ligne du coin inférieur droit"
type: docs
url: /fr/net/aspose.cells.drawing/shape/lowerrightrow/
---
## Shape.LowerRightRow property

Représente l'index de ligne du coin inférieur droit.

```csharp
public int LowerRightRow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Définir et démontrer la propriété LowerRightRow
            Console.WriteLine("Original LowerRightRow: " + shape.LowerRightRow);
            shape.LowerRightRow = 3;
            Console.WriteLine("Modified LowerRightRow: " + shape.LowerRightRow);

            // Modification conditionnelle selon le cas de test
            if (shape.LowerRightRow == 3)
            {
                shape.LowerRightRow = 1;
                Console.WriteLine("Final LowerRightRow after condition: " + shape.LowerRightRow);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


