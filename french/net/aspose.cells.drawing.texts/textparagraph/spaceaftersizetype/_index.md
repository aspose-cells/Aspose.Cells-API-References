---
title: "TextParagraph.SpaceAfterSizeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Obtient et définit la quantité d'espace blanc vertical qui sera présent après un paragraphe"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/
---
## TextParagraph.SpaceAfterSizeType property

Obtient et définit la quantité d'espace blanc vertical qui sera présent après un paragraphe.

```csharp
public LineSpaceSizeType SpaceAfterSizeType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceAfterSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une zone de texte et définir le texte avec plusieurs paragraphes
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Obtenir le deuxième paragraphe
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Définir les propriétés d'espacement avec le type de taille
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceAfter = 10; // 10 points space after
            
            // Enregistrez et rechargez pour vérifier
            string filePath = "TextParagraphPropertySpaceAfterSizeTypeDemo_Output.xlsx";
            workbook.Save(filePath);
            
            Workbook loadedWorkbook = new Workbook(filePath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceAfterSizeType: " + loadedParagraph.SpaceAfterSizeType);
            Console.WriteLine("SpaceAfter: " + loadedParagraph.SpaceAfter);
        }
    }
}
```

### Voir aussi

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


