---
title: "TextOptions.LatinName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextOptions egenskap. Hämtar och anger det latin-namnet"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textoptions/latinname/
---
## TextOptions.LatinName property

Hämtar och anger det latinska namnet.

```csharp
public string LatinName { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera textalternativ
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.Text = "Sample Text";

            // Hämta TextOptions från formens första stycke
            TextOptions textOptions = shape.TextBody.TextParagraphs[0].TextOptions;

            // Visa aktuellt LatinName‑värde
            Console.WriteLine("Current LatinName value: " + textOptions.LatinName);

            // Ange ett nytt LatinName‑värde
            textOptions.LatinName = "Times New Roman";

            // Skapa en annan form för att jämföra typsnittsrendering
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 3, 0, 100, 150);
            shape2.Text = "Comparison Text";
            shape2.TextBody.TextParagraphs[0].TextOptions.LatinName = "Arial";

            // Spara arbetsboken för att se effekterna
            workbook.Save("PropertyLatinNameDemo.xlsx");

            // Visa det nya LatinName‑värdet
            Console.WriteLine("New LatinName value: " + textOptions.LatinName);
        }
    }
}
```

### Se även

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


