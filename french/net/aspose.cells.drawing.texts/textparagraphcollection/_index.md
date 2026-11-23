---
title: "Classe TextParagraphCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Texts.TextParagraphCollection. Représente tous les paragraphes de texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraphcollection/
---
## TextParagraphCollection class

Représente tous les paragraphes de texte.

```csharp
public class TextParagraphCollection : IEnumerable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells.drawing.texts/textparagraphcollection/count/) { get; } | Obtient le nombre de paragraphes de texte. |
| [Item](../../aspose.cells.drawing.texts/textparagraphcollection/item/) { get; } | Obtient l'objet [`TextParagraph`](../textparagraph/) à un indice spécifique. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetEnumerator](../../aspose.cells.drawing.texts/textparagraphcollection/getenumerator/)() | Obtient l'énumérateur des paragraphes. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphCollectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez une zone de texte à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            
            // Définir du texte multi-lignes
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Obtenir la collection de paragraphes
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Accéder et modifier le deuxième paragraphe
            TextParagraph secondParagraph = paragraphs[1];
            secondParagraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            secondParagraph.LineSpace = 20;
            secondParagraph.SpaceAfter = 30;
            secondParagraph.SpaceBefore = 40;
            
            // Enregistrez le classeur
            workbook.Save("TextParagraphCollectionDemo.xlsx");
            
            Console.WriteLine("Text paragraph formatting saved successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


