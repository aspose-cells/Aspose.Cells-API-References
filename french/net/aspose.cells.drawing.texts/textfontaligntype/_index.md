---
title: "Énumération TextFontAlignType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.Texts.TextFontAlignType. Représente les différents types d'alignement de police"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textfontaligntype/
---
## TextFontAlignType enumeration

Représente les différents types d'alignement de police.

```csharp
public enum TextFontAlignType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Automatic | `0` | Lorsque le flux de texte est horizontal ou vertical simple, il est identique à fontBaseline, mais pour les autres modes verticaux, il est identique à fontCenter. |
| Bottom | `1` | Les lettres sont ancrées tout en bas d'une seule ligne. |
| Baseline | `2` | Les lettres sont ancrées à la ligne de base inférieure d'une seule ligne. |
| Center | `3` | Les lettres sont ancrées entre les deux lignes de base d'une seule ligne. |
| Top | `4` | Les lettres sont ancrées à la ligne de base supérieure d'une seule ligne. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextFontAlignTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des zones de texte avec différents alignements de police
            var textBoxAuto = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            textBoxAuto.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Automatic;
            textBoxAuto.Text = "Automatic Alignment";

            var textBoxBottom = worksheet.Shapes.AddTextBox(0, 200, 100, 100, 200, 200);
            textBoxBottom.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Bottom;
            textBoxBottom.Text = "Bottom Alignment";

            var textBoxBaseline = worksheet.Shapes.AddTextBox(0, 400, 100, 100, 200, 200);
            textBoxBaseline.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Baseline;
            textBoxBaseline.Text = "Baseline Alignment";

            var textBoxCenter = worksheet.Shapes.AddTextBox(200, 0, 100, 100, 200, 200);
            textBoxCenter.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Center;
            textBoxCenter.Text = "Center Alignment";

            var textBoxTop = worksheet.Shapes.AddTextBox(200, 200, 100, 100, 200, 200);
            textBoxTop.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Top;
            textBoxTop.Text = "Top Alignment";

            // Afficher toutes les valeurs d'énumération dans la console
            Console.WriteLine("TextFontAlignType values:");
            Console.WriteLine($"Automatic: {TextFontAlignType.Automatic}");
            Console.WriteLine($"Bottom: {TextFontAlignType.Bottom}");
            Console.WriteLine($"Baseline: {TextFontAlignType.Baseline}");
            Console.WriteLine($"Center: {TextFontAlignType.Center}");
            Console.WriteLine($"Top: {TextFontAlignType.Top}");

            // Enregistrez le classeur
            workbook.Save("TextFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


