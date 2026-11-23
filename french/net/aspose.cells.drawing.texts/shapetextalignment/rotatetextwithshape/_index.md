---
title: "ShapeTextAlignment.RotateTextWithShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Indique si le texte tourne avec la forme"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/
---
## ShapeTextAlignment.RotateTextWithShape property

Indique si le texte tourne avec la forme.

```csharp
public bool RotateTextWithShape { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotateTextWithShapeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Accéder aux propriétés d'alignement du texte
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            
            // Définir la propriété RotateTextWithShape
            textAlignment.RotateTextWithShape = true;

            // Faites pivoter la forme pour démontrer l'effet
            shape.RotationAngle = 45;

            // Enregistrez le classeur
            workbook.Save("RotateTextWithShapeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


