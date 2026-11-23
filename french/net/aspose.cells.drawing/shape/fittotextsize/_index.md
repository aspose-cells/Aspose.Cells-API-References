---
title: "Shape.FitToTextSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Recalculer une zone de texte adaptée à l'affichage de tout le contenu textuel"
type: docs
url: /fr/net/aspose.cells.drawing/shape/fittotextsize/
---
## Shape.FitToTextSize method

Recalculer une zone de texte adaptée à l'affichage de tout le contenu texte.

```csharp
public void FitToTextSize()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeMethodFitToTextSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 100);
            textBox.Text = "This is a sample text that will demonstrate the FitToTextSize method functionality.";

            try
            {
                // Afficher les dimensions d'origine
                Console.WriteLine($"Original Width: {textBox.Width}, Height: {textBox.Height}");

                // Appeler la méthode FitToTextSize
                textBox.FitToTextSize();

                // Afficher les dimensions ajustées
                Console.WriteLine($"Adjusted Width: {textBox.Width}, Height: {textBox.Height}");
                Console.WriteLine("FitToTextSize method executed successfully");

                // Ajouter plus de texte pour montrer l'effet
                textBox.Text += " Adding more text to show how the shape adjusts to fit the content.";
                textBox.FitToTextSize();
                Console.WriteLine($"Final Width: {textBox.Width}, Height: {textBox.Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FitToTextSize method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("ShapeMethodFitToTextSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


