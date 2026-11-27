---
title: "Shape.FitToTextSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Beräkna om ett textområde som är lämpligt för att visa allt textinnehåll"
type: docs
url: /sv/net/aspose.cells.drawing/shape/fittotextsize/
---
## Shape.FitToTextSize method

Beräkna om ett textområde som är lämpligt för att visa allt textinnehåll.

```csharp
public void FitToTextSize()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 100);
            textBox.Text = "This is a sample text that will demonstrate the FitToTextSize method functionality.";

            try
            {
                // Visa ursprungliga dimensioner
                Console.WriteLine($"Original Width: {textBox.Width}, Height: {textBox.Height}");

                // Anropa metoden FitToTextSize
                textBox.FitToTextSize();

                // Visa justerade dimensioner
                Console.WriteLine($"Adjusted Width: {textBox.Width}, Height: {textBox.Height}");
                Console.WriteLine("FitToTextSize method executed successfully");

                // Lägg till mer text för att visa effekten
                textBox.Text += " Adding more text to show how the shape adjusts to fit the content.";
                textBox.FitToTextSize();
                Console.WriteLine($"Final Width: {textBox.Width}, Height: {textBox.Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FitToTextSize method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("ShapeMethodFitToTextSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


