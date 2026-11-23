---
title: "TextParagraphCollection.GetEnumerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode TextParagraphCollection. Obtient l'énumérateur des paragraphes"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraphcollection/getenumerator/
---
## TextParagraphCollection.GetEnumerator method

Obtient l'énumérateur des paragraphes.

```csharp
public IEnumerator GetEnumerator()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.Collections;

    public class TextParagraphCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul avec tous les paramètres requis
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 200, 100, 100);
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Obtenez la collection de paragraphes de texte
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;

            try
            {
                // Appelez la méthode GetEnumerator
                IEnumerator enumerator = paragraphs.GetEnumerator();

                Console.WriteLine($"Number of paragraphs: {paragraphs.Count}");
                Console.WriteLine("Paragraphs:");

                // Parcourez les paragraphes à l'aide de l'énumérateur
                while (enumerator.MoveNext())
                {
                    TextParagraph paragraph = (TextParagraph)enumerator.Current;
                    Console.WriteLine(textBox.Text); // Using the text from the textbox since TextParagraph doesn't have Text property
                }

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


