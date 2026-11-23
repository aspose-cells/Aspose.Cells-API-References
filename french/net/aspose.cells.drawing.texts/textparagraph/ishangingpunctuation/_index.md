---
title: "TextParagraph.IsHangingPunctuation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Spécifie si la ponctuation doit être forcée à se placer sur la même ligne de texte ou mise sur une ligne différente"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/
---
## TextParagraph.IsHangingPunctuation property

Spécifie si la ponctuation doit être forcée à se placer sur une ligne de texte ou mise sur une ligne de texte différente.

```csharp
public bool IsHangingPunctuation { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsHangingPunctuationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul (corrigé en ajoutant le paramètre de hauteur)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 100, 200, 100);
            textBox.Text = "This is a sample text with punctuation: \"Hello, world!\"";

            // Obtenir le paragraphe de texte de la zone de texte (corrigé en castant en TextParagraph)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Afficher la valeur actuelle de IsHangingPunctuation
            Console.WriteLine("Current IsHangingPunctuation value: " + textParagraph.IsHangingPunctuation);

            // Définir IsHangingPunctuation sur true
            textParagraph.IsHangingPunctuation = true;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // Définir IsHangingPunctuation sur false
            textParagraph.IsHangingPunctuation = false;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // Enregistrer le classeur pour voir les effets (inspection visuelle requise)
            workbook.Save("TextParagraphPropertyIsHangingPunctuationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


