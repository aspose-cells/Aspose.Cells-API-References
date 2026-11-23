---
title: "TextParagraph.SpaceAfter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Obtient et définit la quantité d'espace blanc vertical qui sera présent après un paragraphe"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/spaceafter/
---
## TextParagraph.SpaceAfter property

Obtient et définit la quantité d'espace blanc vertical qui sera présent après un paragraphe.

```csharp
public double SpaceAfter { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceAfterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une zone de texte et définir le texte
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Obtenir les paragraphes
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Configurer l'espacement du deuxième paragraphe
            TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3; // Demonstrate SpaceAfter property
            p.SpaceBefore = 4;
            
            // Enregistrer et vérifier
            workbook.Save("TextParagraphPropertySpaceAfterDemo.xlsx");
            
            // Recharger pour vérifier les paramètres
            Workbook loadedWorkbook = new Workbook("TextParagraphPropertySpaceAfterDemo.xlsx");
            TextParagraph loadedPara = loadedWorkbook.Worksheets[0].Shapes[0].TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceAfter: " + loadedPara.SpaceAfter);
            Console.WriteLine("SpaceBefore: " + loadedPara.SpaceBefore);
            Console.WriteLine("LineSpace: " + loadedPara.LineSpace);
        }
    }
}
```

### Voir aussi

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


