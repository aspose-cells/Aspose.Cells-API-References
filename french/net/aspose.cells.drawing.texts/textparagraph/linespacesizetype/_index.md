---
title: "TextParagraph.LineSpaceSizeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Obtient et définit la quantité d'espace blanc vertical qui sera utilisé dans un paragraphe"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/linespacesizetype/
---
## TextParagraph.LineSpaceSizeType property

Obtient et définit la quantité d'espace blanc vertical qui sera utilisé dans un paragraphe.

```csharp
public LineSpaceSizeType LineSpaceSizeType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une zone de texte et définir le texte
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // Obtenir le deuxième paragraphe
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Définir les propriétés d'interligne
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2;
            paragraph.SpaceAfter = 3;
            paragraph.SpaceBefore = 4;
            
            // Enregistrer et exporter
            workbook.Save("TextParagraphPropertyLineSpaceSizeTypeDemo_output.xlsx");
            
            Console.WriteLine("Demo executed successfully. Output file created.");
        }
    }
}
```

### Voir aussi

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


