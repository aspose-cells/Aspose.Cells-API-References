---
title: "Style.SetTwoColorGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style‑metod. Anger den angivna fyllningen till en tvåfärgsgradient"
type: docs
url: /sv/net/aspose.cells/style/settwocolorgradient/
---
## Style.SetTwoColorGradient method

Ställer in den angivna fyllningen till en tvåfärgad gradient.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color1 | Färg | En gradientfärg. |
| color2 | Färg | Två gradientfärger. |
| gradientStyleType | GradientStyleType | Gradientskuggningsstil. |
| variant | Int32 | Gradientvarianten. Kan vara ett värde från 1 till 4, motsvarande en av de fyra varianterna på fliken Gradient i dialogrutan Fylleffekter. Om stil är GradientStyle.FromCenter, kan Variant‑argumentet endast vara 1 eller 2. |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett stilobjekt
            Style style = workbook.CreateStyle();

            // Ställ in tvåfärgsgradient för stilen
            style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);

            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Gradient Style Demo");

            // Verifiera gradientinställningarna
            Color color1, color2;
            GradientStyleType gradientStyle;
            int variant;
            style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);

            Console.WriteLine("Color1: " + color1);
            Console.WriteLine("Color2: " + color2);
            Console.WriteLine("Gradient Style: " + gradientStyle);
            Console.WriteLine("Variant: " + variant);

            // Spara arbetsboken
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


