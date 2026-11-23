---
title: "TextParagraph.SpaceBeforeSizeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Obtient et définit la quantité d'espace blanc vertical qui sera présent avant un paragraphe"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/
---
## TextParagraph.SpaceBeforeSizeType property

Obtient et définit la quantité d'espace blanc vertical qui sera présent avant un paragraphe.

```csharp
public LineSpaceSizeType SpaceBeforeSizeType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceBeforeSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez une zone de texte et obtenez sa forme
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Accédez au deuxième paragraphe
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Définissez les propriétés d'espacement du paragraphe
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceBeforeSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            paragraph.LineSpace = 12;
            paragraph.SpaceBefore = 8;
            paragraph.SpaceAfter = 10;
            
            // Enregistrer et recharger pour démontrer la persistance
            string outputPath = "TextParagraphSpacingDemo.xlsx";
            workbook.Save(outputPath);
            
            // Recharger pour vérifier les propriétés
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceBeforeSizeType: " + loadedParagraph.SpaceBeforeSizeType);
            Console.WriteLine("SpaceBefore: " + loadedParagraph.SpaceBefore);
            Console.WriteLine("SpaceAfterSizeType: " + loadedParagraph.SpaceAfterSizeType);
            Console.WriteLine("SpaceAfter: " + loadedParagraph.SpaceAfter);
            Console.WriteLine("LineSpaceSizeType: " + loadedParagraph.LineSpaceSizeType);
            Console.WriteLine("LineSpace: " + loadedParagraph.LineSpace);
        }
    }
}
```

### Voir aussi

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


