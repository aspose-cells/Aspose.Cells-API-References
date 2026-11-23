---
title: "ShapeTextAlignment.TextVerticalType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Obtient et définit la direction du texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/textverticaltype/
---
## ShapeTextAlignment.TextVerticalType property

Obtient et définit la direction du texte.

```csharp
public TextVerticalType TextVerticalType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Obtenez l'alignement du texte et définissez le type de texte vertical
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            textAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Enregistrez le classeur
            workbook.Save("TextVerticalTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextVerticalType](../../textverticaltype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


