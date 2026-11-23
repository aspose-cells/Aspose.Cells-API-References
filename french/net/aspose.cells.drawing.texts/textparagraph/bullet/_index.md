---
title: "TextParagraph.Bullet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Obtient la puce"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/bullet/
---
## TextParagraph.Bullet property

Obtient la puce.

```csharp
public Bullet Bullet { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyBulletDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Définir le texte et configurer le paragraphe
            textbox.Text = "First Item\nSecond Item";
            textbox.TextBody.TextParagraphs[0].LineSpaceSizeType = LineSpaceSizeType.Percentage;
            textbox.TextBody.TextParagraphs[0].LineSpace = 3000;

            // Configurer la puce pour le premier paragraphe
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Enregistrez le classeur
            workbook.Save("TextParagraphPropertyBulletDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Bullet](../../bullet/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


