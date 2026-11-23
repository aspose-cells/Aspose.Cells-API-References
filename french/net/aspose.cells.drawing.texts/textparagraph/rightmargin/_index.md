---
title: "TextParagraph.RightMargin"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Spécifie la marge droite du paragraphe"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/rightmargin/
---
## TextParagraph.RightMargin property

Spécifie la marge droite du paragraphe.

```csharp
public double RightMargin { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "This is a sample text to demonstrate RightMargin property of TextParagraph.";

            // Obtenir le paragraphe de texte du premier paragraphe de la zone de texte
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Afficher la valeur actuelle de la marge droite
            Console.WriteLine("Current RightMargin value: " + paragraph.RightMargin);

            // Définir une nouvelle valeur de marge droite (en points)
            paragraph.RightMargin = 20.0;

            // Ajouter une autre zone de texte pour montrer la différence
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 2, 1, 2, 200, 200);
            textBox2.Text = "This text has default RightMargin for comparison.";
            
            // Enregistrer le classeur pour voir l'effet
            workbook.Save("TextParagraphRightMarginDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


