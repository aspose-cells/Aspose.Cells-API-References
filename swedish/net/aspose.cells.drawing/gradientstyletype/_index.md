---
title: "Enum GradientStyleType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.GradientStyleType enum. Representerar gradientskuggningsstil"
type: docs
url: /sv/net/aspose.cells.drawing/gradientstyletype/
---
## GradientStyleType enumeration

Representerar skuggningsstil för gradient.

```csharp
public enum GradientStyleType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| DiagonalDown | `0` | Diagonal nedåtriktad skuggningsstil |
| DiagonalUp | `1` | Diagonal uppåtriktad skuggningsstil |
| FromCenter | `2` | Från centrum skuggningsstil |
| FromCorner | `3` | Från hörn skuggningsstil |
| Horizontal | `4` | Horisontell skuggningsstil |
| Vertical | `5` | Vertikal skuggningsstil |
| Unknown | `6` | Okänd skuggningsstil. Endast för skuggningsstilen (som inte är någon medlem av GradientStyleType) i mallfilen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStyleTypeDemo
    {
        public static void GradientStyleTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Åtkomst till diagrammets plotområde
            PlotArea plotArea = chart.PlotArea;

            // Åtkomst till fyllformatet för plotområdet
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // Ställ in en tvåfärgsgradientfyllning med DiagonalDown-stil
            fillFormat.SetTwoColorGradient(Color.Blue, Color.White, GradientStyleType.DiagonalDown, 1);

            // Skriv ut den använda gradientstilen
            Console.WriteLine("Gradient Style: " + fillFormat.GradientStyle);

            // Spara arbetsboken
            workbook.Save("GradientStyleTypeExample.xlsx");
            workbook.Save("GradientStyleTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


