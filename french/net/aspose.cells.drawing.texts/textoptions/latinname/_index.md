---
title: "TextOptions.LatinName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextOptions. Obtient et définit le nom latin"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textoptions/latinname/
---
## TextOptions.LatinName property

Obtient et définit le nom latin.

```csharp
public string LatinName { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyLatinNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme pour démontrer les options de texte
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.Text = "Sample Text";

            // Obtenez les TextOptions du premier paragraphe de la forme
            TextOptions textOptions = shape.TextBody.TextParagraphs[0].TextOptions;

            // Affichez la valeur actuelle de LatinName
            Console.WriteLine("Current LatinName value: " + textOptions.LatinName);

            // Définissez une nouvelle valeur pour LatinName
            textOptions.LatinName = "Times New Roman";

            // Créez une autre forme pour comparer le rendu des polices
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 3, 0, 100, 150);
            shape2.Text = "Comparison Text";
            shape2.TextBody.TextParagraphs[0].TextOptions.LatinName = "Arial";

            // Enregistrer le classeur pour voir les effets
            workbook.Save("PropertyLatinNameDemo.xlsx");

            // Affichez la nouvelle valeur de LatinName
            Console.WriteLine("New LatinName value: " + textOptions.LatinName);
        }
    }
}
```

### Voir aussi

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


