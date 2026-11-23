---
title: "TextParagraph.LeftMargin"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Spécifie la marge gauche du paragraphe"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/leftmargin/
---
## TextParagraph.LeftMargin property

Spécifie la marge gauche du paragraphe.

```csharp
public double LeftMargin { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 2, 200, 200);
            textBox.Text = "This is a sample text paragraph.\nSecond line of the paragraph.";

            // Obtenir le paragraphe de texte du premier paragraphe de la zone de texte
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Afficher la valeur actuelle de la marge gauche
            Console.WriteLine("Current LeftMargin value: " + paragraph.LeftMargin);

            // Définir une nouvelle valeur de marge gauche (en points)
            paragraph.LeftMargin = 20.0;

            // Démontrer l'effet en ajoutant une autre zone de texte avec la marge par défaut
            TextBox textBox2 = worksheet.Shapes.AddTextBox(0, 3, 2, 2, 200, 200);
            textBox2.Text = "This text box has default left margin.\nCompare the indentation.";

            // Enregistrer le classeur pour montrer la différence
            workbook.Save("TextParagraphLeftMarginDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


