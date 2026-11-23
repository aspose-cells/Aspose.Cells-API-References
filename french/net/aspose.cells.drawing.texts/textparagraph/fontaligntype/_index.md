---
title: "TextParagraph.FontAlignType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Détermine où, verticalement, sur une ligne de texte, les mots réels sont positionnés. Cela concerne le placement vertical des caractères par rapport aux lignes de base."
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/fontaligntype/
---
## TextParagraph.FontAlignType property

Détermine où, verticalement, sur une ligne de texte, les mots réels sont positionnés. Cela concerne le placement vertical des caractères par rapport aux lignes de base.

```csharp
public TextFontAlignType FontAlignType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFontAlignTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            int textboxIndex = worksheet.TextBoxes.Add(1, 1, 200, 400);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample Text\nFor Font Alignment Demo";

            // Obtenez le premier paragraphe de la zone de texte
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];

            // Affichez la valeur actuelle de FontAlignType
            Console.WriteLine("Current FontAlignType value: " + paragraph.FontAlignType);

            // Définissez FontAlignType sur Bottom
            paragraph.FontAlignType = TextFontAlignType.Bottom;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Définissez FontAlignType sur Center
            paragraph.FontAlignType = TextFontAlignType.Center;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Définissez FontAlignType sur Top
            paragraph.FontAlignType = TextFontAlignType.Top;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Enregistrer le classeur pour voir les effets
            workbook.Save("TextParagraphPropertyFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextFontAlignType](../../textfontaligntype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


