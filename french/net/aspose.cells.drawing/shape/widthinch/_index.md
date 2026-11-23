---
title: "Shape.WidthInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la largeur de la forme en pouces"
type: docs
url: /fr/net/aspose.cells.drawing/shape/widthinch/
---
## Shape.WidthInch property

Représente la largeur de la forme, en pouces.

```csharp
public double WidthInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Définissez la largeur en pouces
            shape.WidthInch = 3;
            Console.WriteLine("Shape width (inches): " + shape.WidthInch);

            // Modifiez la largeur si la condition est remplie
            if (shape.WidthInch == 3)
            {
                shape.WidthInch = 1;
                Console.WriteLine("Modified shape width (inches): " + shape.WidthInch);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


