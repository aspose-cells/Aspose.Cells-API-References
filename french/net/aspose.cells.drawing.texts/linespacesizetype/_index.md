---
title: "Enum LineSpaceSizeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Texts.LineSpaceSizeType enum. Représente le type d'unité de la taille de l'espacement des lignes"
type: docs
url: /fr/net/aspose.cells.drawing.texts/linespacesizetype/
---
## LineSpaceSizeType enumeration

Représente le type d'unité de la taille de l'espacement des lignes.

```csharp
public enum LineSpaceSizeType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Percentage | `0` | Représente en unité d'un pourcentage de la taille du texte. |
| Points | `1` | Représente en unité de points. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme de zone de texte
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Définir le contenu du texte
            textBox.Text = "Sample Text\nSecond Line";
            
            // Accéder au premier paragraphe de la zone de texte
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
            
            // Définir le type de taille de l'espace après en Points
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            // Définir la valeur de l'espace après (12 points)
            paragraph.SpaceAfter = 12;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Text box with line spacing created successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


