---
title: "TextParagraph.IsLatinLineBreak"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Spécifie si un mot latin peut être coupé en deux et renvoyé à la ligne suivante sans qu'un trait d'union ne soit ajouté"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/islatinlinebreak/
---
## TextParagraph.IsLatinLineBreak property

Spécifie si un mot latin peut être coupé en deux et renvoyé à la ligne suivante sans ajouter de trait d'union.

```csharp
public bool IsLatinLineBreak { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsLatinLineBreakDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul (paramètres corrigés pour inclure la hauteur)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "This is a long Latin text that will demonstrate line breaking behavior when IsLatinLineBreak is set to different values.";

            // Obtenir le paragraphe de texte de la zone de texte (cast explicite ajouté)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = ((TextParagraph)fontSetting);

            // Afficher la valeur actuelle de IsLatinLineBreak
            Console.WriteLine("Current IsLatinLineBreak value: " + textParagraph.IsLatinLineBreak);

            // Définir IsLatinLineBreak sur false (les mots latins ne seront pas coupés en fin de ligne)
            textParagraph.IsLatinLineBreak = false;
            Console.WriteLine("Set IsLatinLineBreak to false - Latin words won't break at line end");
            workbook.Save("LatinLineBreakDisabled.xlsx");

            // Définir IsLatinLineBreak sur true (les mots latins peuvent être coupés en fin de ligne)
            textParagraph.IsLatinLineBreak = true;
            Console.WriteLine("Set IsLatinLineBreak to true - Latin words can break at line end");
            workbook.Save("LatinLineBreakEnabled.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


