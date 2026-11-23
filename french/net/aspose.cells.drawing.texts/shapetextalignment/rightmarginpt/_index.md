---
title: "ShapeTextAlignment.RightMarginPt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Retourne la marge droite en unités de points"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/
---
## ShapeTextAlignment.RightMarginPt property

Renvoie la marge droite en unités de points

```csharp
public double RightMarginPt { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Accédez à l'alignement du texte
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Définir la marge droite en points
            shapeTextAlignment.RightMarginPt = 2.0d;

            // Vérifiez la propriété en récupérant la valeur
            Console.WriteLine("Right Margin in Points: " + shapeTextAlignment.RightMarginPt);
        }
    }
}
```

### Voir aussi

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


