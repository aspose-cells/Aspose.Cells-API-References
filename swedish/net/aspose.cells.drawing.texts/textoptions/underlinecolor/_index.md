---
title: "TextOptions.UnderlineColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextOptions egenskap. Hämtar eller anger färgen på understrykning"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textoptions/underlinecolor/
---
## TextOptions.UnderlineColor property

Hämtar eller anger färgen på understrykning.

```csharp
public CellsColor UnderlineColor { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med text för att demonstrera textalternativ
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Underline Color Demo";
            
            // Hämta TextOptions från formen
            TextOptions textOptions = shape.TextOptions;

            try
            {
                // Visa aktuellt UnderlineColor‑värde
                CellsColor currentColor = textOptions.UnderlineColor;
                Console.WriteLine($"Current UnderlineColor - Type: {currentColor.Type}, Color: {currentColor.Color}");

                // Ange ett nytt UnderlineColor (eftersom egenskapen är läs‑skriv)
                CellsColor newColor = textOptions.UnderlineColor; // Use existing color object
                newColor.Color = System.Drawing.Color.Red;
                textOptions.UnderlineColor = newColor;

                // Aktivera understrykning för att se effekten
                textOptions.Underline = FontUnderlineType.Single;

                // Visa det nya UnderlineColor‑värdet
                Console.WriteLine($"New UnderlineColor - Type: {textOptions.UnderlineColor.Type}, Color: {textOptions.UnderlineColor.Color}");

                // Spara arbetsboken för att se effekten
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

### Se även

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


