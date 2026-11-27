---
title: "TextOptions.Kerning"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextOptions egenskap. Anger den minsta typsnittsstorleken då teckenkerning sker för denna textsekvens"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textoptions/kerning/
---
## TextOptions.Kerning property

Anger den minsta teckensnittsstorleken där teckenavstånd (kerning) kommer att tillämpas för detta textsegment.

```csharp
public double Kerning { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyKerningDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med text för att demonstrera kerning
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Kerning Demonstration Text";

            // Hämta TextOptions för formen
            TextOptions textOptions = shape.TextOptions;

            // Visa det aktuella kerning‑värdet
            Console.WriteLine("Current Kerning value: " + textOptions.Kerning);

            // Ställ in kerning till 12 punkter (minsta teckenstorlek för att kerning ska ske)
            textOptions.Kerning = 12;

            // Ställ in en större teckenstorlek för att observera kerningeffekten
            textOptions.Size = 24;

            // Spara arbetsboken för att se effekten
            workbook.Save("PropertyKerningDemo.xlsx");

            // Skapa en annan form med annan kerning för jämförelse
            var shape2 = worksheet.Shapes.AddTextBox(10, 0, 1, 0, 200, 100);
            shape2.Text = "Comparison Text Without Kerning";
            shape2.TextOptions.Size = 24;
            shape2.TextOptions.Kerning = 0; // No kerning

            // Spara igen med båda exemplen
            workbook.Save("PropertyKerningDemoWithComparison.xlsx");
        }
    }
}
```

### Se även

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


