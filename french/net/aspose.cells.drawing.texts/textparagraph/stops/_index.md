---
title: "TextParagraph.Stops"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Obtient la liste des tabulations"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/stops/
---
## TextParagraph.Stops property

Obtient la liste des tabulations.

```csharp
public TextTabStopCollection Stops { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyStopsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez du texte à une cellule et obtenez ses propriétés de paragraphe de texte
            worksheet.Cells["A1"].PutValue("Sample\tText\tWith\tTabs");
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            shape.Text = "Sample\tText\tWith\tTabs";
            
            // Obtenez le paragraphe de texte
            var textOptions = shape.TextBody.TextParagraphs[0];

            // Affichez le nombre actuel de tabulations
            Console.WriteLine("Current tab stops count: " + textOptions.Stops.Count);

            // Ajoutez de nouvelles tabulations
            textOptions.Stops.Add(TextTabAlignmentType.Left, 50);
            textOptions.Stops.Add(TextTabAlignmentType.Center, 100);
            textOptions.Stops.Add(TextTabAlignmentType.Right, 150);

            // Afficher les tabulations mises à jour
            Console.WriteLine("Updated tab stops count: " + textOptions.Stops.Count);
            for (int i = 0; i < textOptions.Stops.Count; i++)
            {
                Console.WriteLine($"Tab {i+1}: Position={textOptions.Stops[i].TabPosition}, Alignment={textOptions.Stops[i].TabAlignment}");
            }

            // Enregistrer le classeur pour voir l'effet
            workbook.Save("TextParagraphStopsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextTabStopCollection](../../texttabstopcollection/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


