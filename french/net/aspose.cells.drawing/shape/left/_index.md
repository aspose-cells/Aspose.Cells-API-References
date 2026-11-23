---
title: "Shape.Left"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente le décalage horizontal de la forme par rapport à sa colonne de gauche en pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shape/left/
---
## Shape.Left property

Représente le décalage horizontal de la forme depuis sa colonne de gauche, en unité de pixels.

```csharp
public int Left { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme pour démontrer la propriété Left
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Définissez la position initiale Left
            shape.Left = 200;
            Console.WriteLine("Shape Left position: " + shape.Left);

            // Modifiez la position Left de façon conditionnelle
            if (shape.Left == 200)
            {
                shape.Left = 150;
                Console.WriteLine("Adjusted Shape Left position: " + shape.Left);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


