---
title: "TextOptions.UnderlineColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextOptions. Obtient ou définit la couleur du soulignement"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textoptions/underlinecolor/
---
## TextOptions.UnderlineColor property

Obtient ou définit la couleur du soulignement.

```csharp
public CellsColor UnderlineColor { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyUnderlineColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme avec du texte pour démontrer les options de texte
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Underline Color Demo";
            
            // Obtenez les TextOptions de la forme
            TextOptions textOptions = shape.TextOptions;

            try
            {
                // Affichez la valeur actuelle d'UnderlineColor
                CellsColor currentColor = textOptions.UnderlineColor;
                Console.WriteLine($"Current UnderlineColor - Type: {currentColor.Type}, Color: {currentColor.Color}");

                // Définissez un nouveau UnderlineColor (car la propriété est en lecture-écriture)
                CellsColor newColor = textOptions.UnderlineColor; // Use existing color object
                newColor.Color = System.Drawing.Color.Red;
                textOptions.UnderlineColor = newColor;

                // Activez le soulignement pour voir l'effet
                textOptions.Underline = FontUnderlineType.Single;

                // Affichez la nouvelle valeur d'UnderlineColor
                Console.WriteLine($"New UnderlineColor - Type: {textOptions.UnderlineColor.Type}, Color: {textOptions.UnderlineColor.Color}");

                // Enregistrer le classeur pour voir l'effet
                workbook.Save("UnderlineColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


