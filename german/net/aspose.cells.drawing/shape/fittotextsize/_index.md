---
title: "Shape.FitToTextSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Berechnet einen Textbereich neu, der geeignet ist, den gesamten Textinhalt anzuzeigen."
type: docs
url: /de/net/aspose.cells.drawing/shape/fittotextsize/
---
## Shape.FitToTextSize method

Berechne einen Textbereich neu, der geeignet ist, den gesamten Textinhalt anzuzeigen.

```csharp
public void FitToTextSize()
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Textfeldform hinzu
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 100);
            textBox.Text = "This is a sample text that will demonstrate the FitToTextSize method functionality.";

            try
            {
                // Originalabmessungen anzeigen
                Console.WriteLine($"Original Width: {textBox.Width}, Height: {textBox.Height}");

                // Rufen Sie die Methode FitToTextSize auf
                textBox.FitToTextSize();

                // Angepasste Abmessungen anzeigen
                Console.WriteLine($"Adjusted Width: {textBox.Width}, Height: {textBox.Height}");
                Console.WriteLine("FitToTextSize method executed successfully");

                // Fügen Sie mehr Text hinzu, um die Wirkung zu zeigen
                textBox.Text += " Adding more text to show how the shape adjusts to fit the content.";
                textBox.FitToTextSize();
                Console.WriteLine($"Final Width: {textBox.Width}, Height: {textBox.Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FitToTextSize method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("ShapeMethodFitToTextSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


