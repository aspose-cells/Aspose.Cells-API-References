---
title: "TextOptions.Spacing"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextOptions egenskap. Anger avståndet mellan tecken inom ett textsegment"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textoptions/spacing/
---
## TextOptions.Spacing property

Anger avståndet mellan tecken inom ett textsegment.

```csharp
public double Spacing { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 0, 100, 200);
            textBox.Text = "Sample Text with Spacing";

            // Hämta textalternativen för textrutan
            TextOptions textOptions = textBox.TextOptions;

            // Visa det aktuella avståndsvärdet
            Console.WriteLine("Current Spacing value: " + textOptions.Spacing);

            // Ställ in nya avståndsvärden och se effekterna
            textOptions.Spacing = 2.0; // Increased spacing
            Console.WriteLine("Text with increased spacing (2.0)");

            // Spara arbetsboken med första avståndet
            workbook.Save("TextSpacingDemo1.xlsx");

            // Ändra avståndet till ett negativt värde (tecken närmare varandra)
            textOptions.Spacing = -1.0;
            Console.WriteLine("Text with decreased spacing (-1.0)");

            // Spara arbetsboken med andra avståndet
            workbook.Save("TextSpacingDemo2.xlsx");

            // Återställ till standardavstånd
            textOptions.Spacing = 0.0;
            Console.WriteLine("Text with default spacing (0.0)");

            // Spara arbetsboken med standardavstånd
            workbook.Save("TextSpacingDemo3.xlsx");
        }
    }
}
```

### Se även

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


