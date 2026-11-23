---
title: "Shape.WidthScale"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit l'échelle de largeur en pourcentage de la largeur d'image originale. Si la forme n'est pas une image, la propriété WidthScale ne renvoie que 100"
type: docs
url: /fr/net/aspose.cells.drawing/shape/widthscale/
---
## Shape.WidthScale property

Obtient et définit l'échelle de largeur, en pourcentage de la largeur originale de l'image. Si la forme n'est pas une image, la propriété WidthScale ne renvoie que 100 ;

```csharp
public int WidthScale { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un shape rectangle avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Définir l'échelle de largeur initiale
            shape.WidthScale = 50;
            Console.WriteLine("Initial WidthScale: " + shape.WidthScale);

            // Modifier l'échelle de largeur si la condition est remplie
            if (shape.WidthScale == 50)
            {
                shape.WidthScale = 75;
                Console.WriteLine("Updated WidthScale: " + shape.WidthScale);
            }

            // Enregistrez le classeur
            workbook.Save("ShapeWidthScaleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


