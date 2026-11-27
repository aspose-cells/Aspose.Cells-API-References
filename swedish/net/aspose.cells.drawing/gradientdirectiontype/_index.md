---
title: "Enum GradientDirectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.GradientDirectionType enum. Representerar alla riktningstyper för gradient"
type: docs
url: /sv/net/aspose.cells.drawing/gradientdirectiontype/
---
## GradientDirectionType enumeration

Representerar alla riktningstyper för gradient.

```csharp
public enum GradientDirectionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| FromUpperLeftCorner | `0` | FromUpperLeftCorner |
| FromUpperRightCorner | `1` | FromUpperRightCorner |
| FromLowerLeftCorner | `2` | FromLowerLeftCorner |
| FromLowerRightCorner | `3` | FromLowerRightCorner |
| FromCenter | `4` | FromCenter |
| Unknown | `5` | Okänd |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientDirectionTypeDemo
    {
        public static void GradientDirectionTypeExample()
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

            // Ställ in en tvåfärgsgradientfyllning med en specifik riktning
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Skriv ut gradientens riktningstyp
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Spara arbetsboken
            workbook.Save("GradientDirectionTypeExample.xlsx");
            workbook.Save("GradientDirectionTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


