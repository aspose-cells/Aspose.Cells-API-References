---
title: "Enum ShapeTextVerticalAlignmentType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Texts.ShapeTextVerticalAlignmentType enum. Cela correspond à Format Shape  Text Options  Text Box  Vertical Alignment dans Excel"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextverticalalignmenttype/
---
## ShapeTextVerticalAlignmentType enumeration

Il correspond à "Format Shape - Text Options - Text Box - Vertical Alignment" dans Excel.

```csharp
public enum ShapeTextVerticalAlignmentType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Top | `0` |  |
| Middle | `1` |  |
| Bottom | `2` |  |
| TopCentered | `3` |  |
| MiddleCentered | `4` |  |
| BottomCentered | `5` |  |
| Left | `6` |  |
| Center | `7` |  |
| Right | `8` |  |
| LeftMiddle | `9` |  |
| CenterMiddle | `10` |  |
| RightMiddle | `11` |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassShapeTextVerticalAlignmentTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter une zone de texte à la feuille de calcul
                var textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 300);
                textBox.Text = "Sample text for vertical alignment demonstration";

                // Définir l'alignement vertical du texte sur Milieu
                textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;

                // Afficher l'alignement vertical actuel
                Console.WriteLine("Current vertical alignment: " + textBox.TextBoxOptions.ShapeTextVerticalAlignment);

                // Modifier l'alignement en haut
                textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Top;
                Console.WriteLine("Changed to: " + textBox.TextBoxOptions.ShapeTextVerticalAlignment);

                // Enregistrez le classeur
                workbook.Save("ShapeTextVerticalAlignmentTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapeTextVerticalAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


