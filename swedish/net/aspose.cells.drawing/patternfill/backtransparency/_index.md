---
title: "PatternFill.BackTransparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PatternFill-egenskap. Hämtar eller anger genomskinligheten för bakgrundsfärgen"
type: docs
url: /sv/net/aspose.cells.drawing/patternfill/backtransparency/
---
## PatternFill.BackTransparency property

Hämtar eller anger transparensen för bakgrundsfärgen.

```csharp
public double BackTransparency { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform i arbetsbladet
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Hämta den befintliga PatternFill-instansen från formen och konfigurera egenskaperna
            shape.Fill.FillType = FillType.Pattern;
            PatternFill patternFill = shape.Fill.PatternFill;
            patternFill.Pattern = FillPattern.Solid;
            patternFill.BackgroundColor = Color.Blue;

            // Visa det ursprungliga värdet för BackTransparency
            Console.WriteLine("Current BackTransparency value: " + patternFill.BackTransparency);

            // Ange ett nytt värde för BackTransparency (50 % genomskinlighet)
            patternFill.BackTransparency = 0.5;

            // Spara den modifierade arbetsboken
            workbook.Save("PatternFillBackTransparencyDemo.xlsx");
        }
    }
}
```

### Se även

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


