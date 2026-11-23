---
title: "TextOptions.Spacing"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextOptions. Spécifie l'espacement entre les caractères au sein d'une séquence de texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textoptions/spacing/
---
## TextOptions.Spacing property

Spécifie l'espacement entre les caractères au sein d'une séquence de texte.

```csharp
public double Spacing { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertySpacingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 0, 100, 200);
            textBox.Text = "Sample Text with Spacing";

            // Obtenez les options de texte de la zone de texte
            TextOptions textOptions = textBox.TextOptions;

            // Affichez la valeur d'espacement actuelle
            Console.WriteLine("Current Spacing value: " + textOptions.Spacing);

            // Définissez de nouvelles valeurs d'espacement et voyez les effets
            textOptions.Spacing = 2.0; // Increased spacing
            Console.WriteLine("Text with increased spacing (2.0)");

            // Enregistrez le classeur avec le premier espacement
            workbook.Save("TextSpacingDemo1.xlsx");

            // Modifiez l'espacement à une valeur négative (caractères plus rapprochés)
            textOptions.Spacing = -1.0;
            Console.WriteLine("Text with decreased spacing (-1.0)");

            // Enregistrez le classeur avec le deuxième espacement
            workbook.Save("TextSpacingDemo2.xlsx");

            // Réinitialisez à l'espacement par défaut
            textOptions.Spacing = 0.0;
            Console.WriteLine("Text with default spacing (0.0)");

            // Enregistrez le classeur avec l'espacement par défaut
            workbook.Save("TextSpacingDemo3.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


