---
title: "Class TwoColorGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TwoColorGradient-klass. Representerar en tvåfärgsgradient"
type: docs
url: /sv/net/aspose.cells/twocolorgradient/
---
## TwoColorGradient class

Representerar en tvåfärgsgradient.

```csharp
public class TwoColorGradient
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [TwoColorGradient](twocolorgradient/)(Color, Color, GradientStyleType, int) |  |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Color1](../../aspose.cells/twocolorgradient/color1/) { get; set; } | Hämtar och anger den första gradientfärgen. |
| [Color2](../../aspose.cells/twocolorgradient/color2/) { get; set; } | Hämtar och anger den andra gradientfärgen. |
| [GradientStyleType](../../aspose.cells/twocolorgradient/gradientstyletype/) { get; set; } | Hämtar och anger gradientskuggningsstil. |
| [Variant](../../aspose.cells/twocolorgradient/variant/) { get; set; } | Hämtar och anger gradientvarianten. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class CellsClassTwoColorGradientDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Initiera TwoColorGradient med konstruktörsparametrar
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightSkyBlue, 
                Color.DarkBlue, 
                GradientStyleType.DiagonalUp, 
                2);

            // Ändra gradientegenskaper efter initiering
            gradient.GradientStyleType = GradientStyleType.DiagonalDown;

            // Skapa cellstil och tillämpa gradient
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);

            // Tillämpa stil på cellen och lägg till innehåll
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Aspose.Cells TwoColorGradient Demo");
            cell.SetStyle(style);

            // Justera cellens dimensioner för synlighet
            worksheet.Cells.SetRowHeight(1, 45);
            worksheet.Cells.SetColumnWidth(1, 55);

            // Spara resultatet med gradientformatering
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


