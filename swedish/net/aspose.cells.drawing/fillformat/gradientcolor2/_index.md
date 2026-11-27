---
title: "FillFormat.GradientColor2"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Returnerar gradientfärg 2 för den angivna fyllningen"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/gradientcolor2/
---
## FillFormat.GradientColor2 property

Returnerar gradientfärg 2 för den angivna fyllningen.

```csharp
public Color GradientColor2 { get; }
```

### Anmärkningar

Endast när gradientfärgstypen är GradientColorType.TwoColors, är denna egenskap meningsfull.

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientColor2Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa rektangulär form med tvåfärgsgradientfyllning
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fill = rectangle.Fill;
            
            fill.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 2);

            // Verifiera gradientfärgsegenskaper
            Console.WriteLine("GradientColor2: " + fill.GradientColor2);
        }
    }
}
```

### Se även

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


