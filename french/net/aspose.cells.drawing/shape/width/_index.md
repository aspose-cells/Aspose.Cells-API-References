---
title: "Shape.Width"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la largeur de la forme en pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shape/width/
---
## Shape.Width property

Représente la largeur de la forme, en unités de pixels.

```csharp
public int Width { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un shape rectangle avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 50);

            // Définir la largeur initiale et l'afficher
            shape.Width = 300;
            Console.WriteLine("Initial width: " + shape.Width);

            // Modifier la largeur en fonction d'une condition
            if (shape.Width == 300)
                shape.Width = 150;

            Console.WriteLine("Modified width: " + shape.Width);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


