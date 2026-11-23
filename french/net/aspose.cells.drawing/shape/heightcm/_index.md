---
title: "Shape.HeightCM"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la hauteur de la forme en unité de centimètres"
type: docs
url: /fr/net/aspose.cells.drawing/shape/heightcm/
---
## Shape.HeightCM property

Représente la hauteur de la forme, en centimètres.

```csharp
public double HeightCM { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Définir la hauteur en centimètres
            shape.HeightCM = 3;
            Console.WriteLine("Shape height: " + shape.HeightCM + " cm");

            // Modifier la hauteur si elle est de 3 cm
            if (shape.HeightCM == 3)
            {
                shape.HeightCM = 1;
                Console.WriteLine("Modified shape height: " + shape.HeightCM + " cm");
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


