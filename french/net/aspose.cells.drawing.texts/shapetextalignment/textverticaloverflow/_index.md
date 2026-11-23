---
title: "ShapeTextAlignment.TextVerticalOverflow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Obtient et définit le type de dépassement vertical du texte de la zone de texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/
---
## ShapeTextAlignment.TextVerticalOverflow property

Obtient et définit le type de dépassement vertical du texte de la zone de texte.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Définir le texte qui pourrait dépasser verticalement
            shape.Text = "This is a long text that might overflow vertically if not clipped properly";

            // Obtenir l'alignement du texte et définir le dépassement vertical sur Clip
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;

            // Enregistrez le classeur
            workbook.Save("TextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


