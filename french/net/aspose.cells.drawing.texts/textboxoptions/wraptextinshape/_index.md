---
title: "TextBoxOptions.WrapTextInShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxOptions. Spécifie le retour à la ligne du texte à l'intérieur d'une forme. False  Aucun retour à la ligne ne se produira sur le corps du texte. True  Un retour à la ligne se produira sur le corps du texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textboxoptions/wraptextinshape/
---
## TextBoxOptions.WrapTextInShape property

Spécifie le retour à la ligne du texte dans une forme. False - Aucun retour à la ligne ne se produira dans le corps du texte. True - Le retour à la ligne se produira dans le corps du texte.

```csharp
public bool WrapTextInShape { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyWrapTextInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte avec les paramètres corrects
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Définir le texte qui sera renvoyé à la ligne à l'intérieur de la forme
            textBox.Text = "This is a long text that should wrap within the text box shape boundaries when WrapTextInShape is enabled.";

            // Activer le retour à la ligne du texte à l'intérieur de la forme
            textBox.TextBoxOptions.WrapTextInShape = true;

            // Enregistrez le classeur
            workbook.Save("TextBoxWrapTextDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


