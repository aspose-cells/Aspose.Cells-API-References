---
title: "TextTabStopCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "méthode TextTabStopCollection. Ajoute un arrêt de tabulation"
type: docs
url: /fr/net/aspose.cells.drawing.texts/texttabstopcollection/add/
---
## TextTabStopCollection.Add method

Ajoute une tabulation.

```csharp
public int Add(TextTabAlignmentType tabAlignment, double tabPosition)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tabAlignment | TextTabAlignmentType |  |
| tabPosition | Double |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionMethodAddWithTextTabAlignmentTypeDoubleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour ajouter du texte avec des arrêts de tabulation
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            var textParagraph = shape.TextBody.TextParagraphs[0];
            
            // Obtenir la TextTabStopCollection
            var tabStops = textParagraph.Stops;

            try
            {
                // Appeler la méthode Add avec TextTabAlignmentType.Left et la position 50.0
                int index1 = tabStops.Add(TextTabAlignmentType.Left, 50.0);
                
                // Appeler la méthode Add avec TextTabAlignmentType.Right et la position 100.0
                int index2 = tabStops.Add(TextTabAlignmentType.Right, 100.0);
                
                // Ajouter du texte avec des tabulations pour démontrer les arrêts de tabulation
                shape.Text = "Left-aligned\tRight-aligned";

                Console.WriteLine("Added tab stops at positions 50.0 (Left) and 100.0 (Right)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("TextTabStopCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextTabAlignmentType](../../texttabalignmenttype/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


