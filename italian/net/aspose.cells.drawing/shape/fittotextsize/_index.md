---
title: "Shape.FitToTextSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Ricalcola un'area di testo adatta a visualizzare tutto il contenuto testuale"
type: docs
url: /it/net/aspose.cells.drawing/shape/fittotextsize/
---
## Shape.FitToTextSize method

Ricalcola un'area di testo adatta a visualizzare tutto il contenuto testuale.

```csharp
public void FitToTextSize()
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di casella di testo
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 100);
            textBox.Text = "This is a sample text that will demonstrate the FitToTextSize method functionality.";

            try
            {
                // Visualizza le dimensioni originali
                Console.WriteLine($"Original Width: {textBox.Width}, Height: {textBox.Height}");

                // Chiama il metodo FitToTextSize
                textBox.FitToTextSize();

                // Visualizza le dimensioni regolate
                Console.WriteLine($"Adjusted Width: {textBox.Width}, Height: {textBox.Height}");
                Console.WriteLine("FitToTextSize method executed successfully");

                // Aggiungi più testo per mostrare l'effetto
                textBox.Text += " Adding more text to show how the shape adjusts to fit the content.";
                textBox.FitToTextSize();
                Console.WriteLine($"Final Width: {textBox.Width}, Height: {textBox.Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FitToTextSize method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("ShapeMethodFitToTextSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


