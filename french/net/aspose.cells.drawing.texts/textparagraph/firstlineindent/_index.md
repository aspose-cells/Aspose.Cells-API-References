---
title: "TextParagraph.FirstLineIndent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Spécifie la taille du retrait qui sera appliquée à la première ligne de texte du paragraphe"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/firstlineindent/
---
## TextParagraph.FirstLineIndent property

Spécifie la taille du retrait qui sera appliquée à la première ligne de texte du paragraphe.

```csharp
public double FirstLineIndent { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFirstLineIndentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 100, 300, 200, 100);
            textBox.Text = "This is a sample paragraph with multiple lines.\nFirst line should have indent.\nSecond line should be normal.";

            // Obtenir le paragraphe de texte depuis la zone de texte
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Afficher la valeur actuelle de FirstLineIndent
            Console.WriteLine("Current FirstLineIndent value: " + textParagraph.FirstLineIndent);

            // Définir une nouvelle valeur de FirstLineIndent (20 points)
            textParagraph.FirstLineIndent = 20;
            Console.WriteLine("FirstLineIndent set to: " + textParagraph.FirstLineIndent);

            // Ajouter une autre zone de texte pour comparer avec le retrait par défaut
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 5, 150, 300, 200, 100);
            textBox2.Text = "This is a comparison paragraph without indent.\nFirst line has no indent.\nSecond line is normal.";

            // Enregistrer le classeur pour voir les effets
            workbook.Save("TextParagraphPropertyFirstLineIndentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


