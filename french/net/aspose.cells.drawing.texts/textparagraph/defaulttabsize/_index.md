---
title: "TextParagraph.DefaultTabSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraph. Obtient et définit la taille par défaut d'un caractère de tabulation dans ce paragraphe"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/defaulttabsize/
---
## TextParagraph.DefaultTabSize property

Obtient et définit la taille par défaut d'un caractère de tabulation dans ce paragraphe.

```csharp
public double DefaultTabSize { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyDefaultTabSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 200);
            textBox.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Obtenir le paragraphe de texte du premier paragraphe de la zone de texte
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Afficher la taille de tabulation par défaut actuelle
            Console.WriteLine("Current DefaultTabSize: " + paragraph.DefaultTabSize);

            // Définir une taille d'onglet plus petite (la valeur par défaut est généralement d'environ 36 points)
            paragraph.DefaultTabSize = 20.0;
            Console.WriteLine("DefaultTabSize set to: " + paragraph.DefaultTabSize);

            // Ajouter une autre zone de texte avec la taille d'onglet par défaut pour la comparaison
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 3, 1, 3, 300, 200);
            textBox2.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Enregistrer le classeur pour voir la différence d'espacement des onglets
            workbook.Save("TextParagraphDefaultTabSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


