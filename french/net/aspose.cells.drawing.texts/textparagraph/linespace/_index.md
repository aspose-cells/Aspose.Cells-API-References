---
title: "TextParagraph.LineSpace"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Obtient et définit la quantité d'espace blanc vertical qui sera utilisé dans un paragraphe"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/linespace/
---
## TextParagraph.LineSpace property

Obtient et définit la quantité d'espace blanc vertical qui sera utilisé dans un paragraphe.

```csharp
public double LineSpace { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyLineSpaceDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme de zone de texte
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // Accédez aux paragraphes de texte
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Configurer l'espacement des lignes pour le deuxième paragraphe
            TextParagraph paragraph = paragraphs[1];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2; // Set line spacing to 2 points
            
            // Enregistrer et recharger pour démontrer la persistance
            string outputPath = "output_LineSpaceDemo.xlsx";
            workbook.Save(outputPath);
            
            // Recharger pour vérifier les paramètres
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("Line space: " + loadedParagraph.LineSpace);
            Console.WriteLine("Line space type: " + loadedParagraph.LineSpaceSizeType);
        }
    }
}
```

### Voir aussi

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


