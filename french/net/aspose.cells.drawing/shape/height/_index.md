---
title: "Shape.Height"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la hauteur de la forme en pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shape/height/
---
## Shape.Height property

Représente la hauteur de la forme, en unités de pixel.

```csharp
public int Height { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Définir la hauteur initiale
            shape.Height = 150;
            Console.WriteLine("Initial height: " + shape.Height);

            // Modifier la hauteur de manière conditionnelle
            if (shape.Height == 150)
            {
                shape.Height = 100;
                Console.WriteLine("Modified height: " + shape.Height);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


