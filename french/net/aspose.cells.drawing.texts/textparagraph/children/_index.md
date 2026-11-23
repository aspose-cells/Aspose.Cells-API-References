---
title: "TextParagraph.Children"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Obtient toutes les séquences de texte dans ce paragraphe. Si ce paragraphe est vide, renvoie le paragraphe lui‑même"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/children/
---
## TextParagraph.Children property

Obtient toutes les séquences de texte dans ce paragraphe. Si ce paragraphe est vide, renvoie le paragraphe lui‑même.

```csharp
public FontSetting[] Children { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyChildrenDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 100, 200);
            textBox.Text = "First line\nSecond line\nThird line";

            // Obtenir la collection de paragraphes de texte
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Afficher le nombre d'enfants (séquences de texte) dans le paragraphe
            Console.WriteLine("Number of children (text runs): " + textParagraph.Children.Length);

            // Modifier les paramètres de police de chaque enfant (séquence de texte)
            foreach (FontSetting child in textParagraph.Children)
            {
                child.Font.Size = 12;
                child.Font.Color = System.Drawing.Color.Blue;
                child.Font.IsBold = true;
            }

            // Ajouter une autre ligne avec un formatage différent
            textBox.Text += "\nFourth line";
            fontSetting = (FontSetting)textBox.GetCharacters()[textBox.Text.Length - 1];
            textParagraph = (TextParagraph)fontSetting;

            // Afficher le nombre mis à jour d'enfants
            Console.WriteLine("Updated number of children: " + textParagraph.Children.Length);

            // Enregistrez le classeur
            workbook.Save("TextParagraphChildrenDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


