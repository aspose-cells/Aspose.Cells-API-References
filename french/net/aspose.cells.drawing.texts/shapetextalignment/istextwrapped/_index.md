---
title: "ShapeTextAlignment.IsTextWrapped"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Obtient ou définit le type d'habillage du texte de la forme qui contient du texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/istextwrapped/
---
## ShapeTextAlignment.IsTextWrapped property

Obtient ou définit le type d'enroulement du texte de la forme qui contient du texte.

```csharp
public bool IsTextWrapped { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Définissez le texte de la forme
            shape.Text = "This is a long text that should be wrapped when IsTextWrapped is set to true";

            // Obtenir l'alignement du texte et définir IsTextWrapped
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.IsTextWrapped = true;

            // Enregistrez le classeur
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


