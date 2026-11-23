---
title: "TextParagraph.IsEastAsianLineBreak"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Spécifie si un mot d'Asie de l'Est peut être coupé en deux et renvoyé à la ligne suivante sans qu'un trait d'union ne soit ajouté"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/
---
## TextParagraph.IsEastAsianLineBreak property

Spécifie si un mot d'Asie de l'Est peut être coupé en deux et renvoyé à la ligne suivante sans ajouter de trait d'union.

```csharp
public bool IsEastAsianLineBreak { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsEastAsianLineBreakDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "これは東アジアのテキストの例です。This is Latin text example.";

            // Obtenir le paragraphe de texte du premier paragraphe de la zone de texte
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Affichez la valeur actuelle de IsEastAsianLineBreak
            Console.WriteLine("Current IsEastAsianLineBreak value: " + paragraph.IsEastAsianLineBreak);

            // Définissez IsEastAsianLineBreak sur false (les mots d'Asie de l'Est peuvent être coupés)
            paragraph.IsEastAsianLineBreak = false;
            Console.WriteLine("After setting IsEastAsianLineBreak to false, text may break East Asian words.");

            // Enregistrez le classeur avec la coupure de ligne d'Asie de l'Est désactivée
            workbook.Save("EastAsianLineBreakDisabled.xlsx");

            // Définissez IsEastAsianLineBreak sur true (les mots d'Asie de l'Est ne seront pas coupés)
            paragraph.IsEastAsianLineBreak = true;
            Console.WriteLine("After setting IsEastAsianLineBreak to true, text won't break East Asian words.");

            // Enregistrez le classeur avec la coupure de ligne d'Asie de l'Est activée
            workbook.Save("EastAsianLineBreakEnabled.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


