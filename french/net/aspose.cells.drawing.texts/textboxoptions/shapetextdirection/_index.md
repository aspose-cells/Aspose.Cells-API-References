---
title: "TextBoxOptions.ShapeTextDirection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxOptions. Obtient ou définit la direction d'affichage du texte au sein d'un corps de texte donné. Elle correspond à Format Shape  Text Options  Text Box  Text direction dans Excel"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textboxoptions/shapetextdirection/
---
## TextBoxOptions.ShapeTextDirection property

Obtient ou définit la direction d'affichage du texte dans un corps de texte donné. Cela correspond à "Format Shape - Text Options - Text Box - Text direction" dans Excel

```csharp
public TextVerticalType ShapeTextDirection { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyShapeTextDirectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Définir la direction du texte en vertical
            shape.TextBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;

            // Définir du texte pour démontrer la direction
            shape.Text = "Vertical Text Example";

            // Enregistrez le classeur
            workbook.Save("TextBoxTextDirectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextVerticalType](../../textverticaltype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


