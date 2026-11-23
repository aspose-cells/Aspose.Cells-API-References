---
title: "Shape.HeightScale"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit l'échelle de hauteur en pourcentage de la hauteur de l'image originale. Si la forme n'est pas une image, la propriété HeightScale renvoie uniquement 100"
type: docs
url: /fr/net/aspose.cells.drawing/shape/heightscale/
---
## Shape.HeightScale property

Obtient et définit l'échelle de hauteur, en pourcentage de la hauteur originale de l'image. Si la forme n'est pas une image, la propriété HeightScale ne renvoie que 100;

```csharp
public int HeightScale { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightScaleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 150);

            // Définir l'échelle de hauteur initiale
            shape.HeightScale = 50;
            Console.WriteLine("Initial HeightScale: " + shape.HeightScale);

            // Modifier l'échelle de hauteur si la condition est remplie
            if (shape.HeightScale == 50)
            {
                shape.HeightScale = 75;
                Console.WriteLine("Modified HeightScale: " + shape.HeightScale);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


