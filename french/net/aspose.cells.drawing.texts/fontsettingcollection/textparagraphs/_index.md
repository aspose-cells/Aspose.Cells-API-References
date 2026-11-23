---
title: "FontSettingCollection.TextParagraphs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FontSettingCollection. Obtient tous les paragraphes"
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/
---
## FontSettingCollection.TextParagraphs property

Obtient tous les paragraphes.

```csharp
public TextParagraphCollection TextParagraphs { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyTextParagraphsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "First paragraph\nSecond paragraph";

            // Accéder au premier paragraphe de texte
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            
            // Définir les propriétés d'interligne
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000; // 300% line spacing

            // Définir les propriétés des puces
            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Enregistrez le classeur
            workbook.Save("TextParagraphsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextParagraphCollection](../../textparagraphcollection/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


