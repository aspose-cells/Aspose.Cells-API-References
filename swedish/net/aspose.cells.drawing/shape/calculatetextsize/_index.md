---
title: "Shape.CalculateTextSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Beräkna om textområdet"
type: docs
url: /sv/net/aspose.cells.drawing/shape/calculatetextsize/
---
## Shape.CalculateTextSize method

Beräkna om textområdet

```csharp
public int[] CalculateTextSize()
```

### Returvärde

Textens storlek i en array (bredd och höjd).

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCalculateTextSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett exempel på text i cell A1
            worksheet.Cells["A1"].PutValue("Sample Text for Size Calculation");

            // Skapa en rektangelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Ställ in text på formen
            shape.Text = "This is a test string to calculate text size";

            // Beräkna textstorleken
            int[] size = shape.CalculateTextSize();

            // Skriv ut resultaten
            Console.WriteLine($"Calculated text size - Width: {size[0]}, Height: {size[1]}");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


