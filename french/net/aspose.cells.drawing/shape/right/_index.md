---
title: "Shape.Right"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la largeur du décalage horizontal de la forme depuis la colonne de son coin inférieur droit, en pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shape/right/
---
## Shape.Right property

Représente la largeur du décalage horizontal de la forme depuis la colonne du coin inférieur droit, en unités de pixels.

```csharp
public int Right { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Définissez et obtenez la propriété Right
            shape.Right = 200;
            Console.WriteLine("Shape Right position: " + shape.Right);

            // Modifiez la propriété Right de façon conditionnelle
            if (shape.Right == 200)
                shape.Right = 150;

            Console.WriteLine("Modified Shape Right position: " + shape.Right);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


