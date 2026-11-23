---
title: "Shape.TextBoxOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Shape property. Obtient les informations texte dans le shape"
type: docs
url: /fr/net/aspose.cells.drawing/shape/textboxoptions/
---
## Shape.TextBoxOptions property

Obtient les informations texte dans la forme

```csharp
public TextBoxOptions TextBoxOptions { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;

    public class ShapePropertyTextBoxOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte
            int textBoxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "This is a sample text box to demonstrate TextBoxOptions properties.";

            // Afficher les propriétés actuelles de TextBoxOptions
            TextBoxOptions textBoxOptions = textBox.TextBoxOptions;
            Console.WriteLine("Current TextBoxOptions:");
            Console.WriteLine("Vertical Alignment: " + textBoxOptions.ShapeTextVerticalAlignment);
            Console.WriteLine("Resize To Fit Text: " + textBoxOptions.ResizeToFitText);
            Console.WriteLine("Text Direction: " + textBoxOptions.ShapeTextDirection);
            Console.WriteLine("Left Margin: " + textBoxOptions.LeftMarginPt + " pt");
            Console.WriteLine("Right Margin: " + textBoxOptions.RightMarginPt + " pt");

            // Modifier les propriétés de TextBoxOptions
            textBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;
            textBoxOptions.ResizeToFitText = true;
            textBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;
            textBoxOptions.LeftMarginPt = 10;
            textBoxOptions.RightMarginPt = 10;
            textBoxOptions.TopMarginPt = 5;
            textBoxOptions.BottomMarginPt = 5;

            // Enregistrez le classeur
            workbook.Save("TextBoxOptionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBoxOptions](../../../aspose.cells.drawing.texts/textboxoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


