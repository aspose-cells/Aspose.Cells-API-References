---
title: "Shape.Bottom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la largeur du décalage vertical de la forme depuis sa rangée d'angle inférieur en unités de pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shape/bottom/
---
## Shape.Bottom property

Représente la largeur du décalage vertical de la forme depuis la rangée du coin inférieur inférieur, en unités de pixels.

```csharp
public int Bottom { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Définir la position initiale
            shape.Top = 200;
            shape.Left = 200;

            // Démontrer la propriété Bottom
            Console.WriteLine("Original Bottom position: " + shape.Bottom);

            // Modifier la position Bottom
            if (shape.Bottom == 300)  // 200 (Top) + 100 (Height)
            {
                shape.Bottom = 250;  // This will change the Top position (250 - 100 = 150)
                Console.WriteLine("New Bottom position: " + shape.Bottom);
                Console.WriteLine("New Top position: " + shape.Top);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


