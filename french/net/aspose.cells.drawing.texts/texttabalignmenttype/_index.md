---
title: "Énumération TextTabAlignmentType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.Texts.TextTabAlignmentType. Représente les types d'alignement des tabulations de texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/texttabalignmenttype/
---
## TextTabAlignmentType enumeration

Représente les types d'alignement des tabulations de texte.

```csharp
public enum TextTabAlignmentType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Center | `0` | Le texte à cet arrêt de tabulation est centré. |
| Decimal | `1` | À cet arrêt de tabulation, les décimales sont alignées. |
| Left | `2` | Le texte à cet arrêt de tabulation est aligné à gauche. |
| Right | `3` | Le texte à cet arrêt de tabulation est aligné à droite. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextTabAlignmentTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une zone de texte pour démontrer les alignements de tabulation
            int textBoxIndex = worksheet.TextBoxes.Add(0, 0, 400, 300);
            var textBox = worksheet.TextBoxes[textBoxIndex];
            var paragraph = textBox.TextBody.TextParagraphs[0];

            // Ajoutez des arrêts de tabulation avec différents types d'alignement
            paragraph.Stops.Add(TextTabAlignmentType.Left, 100);
            paragraph.Stops.Add(TextTabAlignmentType.Center, 200);
            paragraph.Stops.Add(TextTabAlignmentType.Right, 300);
            paragraph.Stops.Add(TextTabAlignmentType.Decimal, 400);

            // Définissez le texte pour démontrer tous les types d'alignement
            textBox.Text = "Left\tCenter\tRight\tDecimal\n" +
                           "Data\tData\tData\t12.34\n" +
                           "More\tMore\tMore\t56.78";

            // Appliquez le formatage pour rendre les tabulations visibles
            textBox.Font.Size = 12;
            textBox.TextBody.TextParagraphs[0].AlignmentType = TextAlignmentType.Left;

            // Enregistrer le résultat
            workbook.Save("TextTabAlignmentTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


