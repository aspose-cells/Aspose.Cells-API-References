---
title: "Enum TrendlineType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.TrendlineType enum. Representerar trendline-typen"
type: docs
url: /sv/net/aspose.cells.charts/trendlinetype/
---
## TrendlineType enumeration

Representerar trendlinjetypen.

```csharp
public enum TrendlineType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Exponential | `0` | Exponentiell |
| Linear | `1` | Linjär |
| Logarithmic | `2` | Logaritmisk |
| MovingAverage | `3` | Rullande medelvärde |
| Polynomial | `4` | Polynom |
| Power | `5` | Potens |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineTypeDemo
    {
        public static void TrendlineTypeExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Lägger till ett nytt kalkylblad i Excel-objektet
            int sheetIndex = workbook.Worksheets.Add();
            
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Lägger till exempelvärden i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägger till NSeries (diagramdatakälla) i diagrammet från cellen "A1" till "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Anger datakällan för kategoridata i NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Lägga till olika typer av trendlines i diagrammet
            AddTrendline(chart, 0, TrendlineType.Linear, "Linear Trendline");
            AddTrendline(chart, 0, TrendlineType.Exponential, "Exponential Trendline");
            AddTrendline(chart, 0, TrendlineType.Logarithmic, "Logarithmic Trendline");
            AddTrendline(chart, 0, TrendlineType.MovingAverage, "Moving Average Trendline");
            AddTrendline(chart, 0, TrendlineType.Polynomial, "Polynomial Trendline");
            AddTrendline(chart, 0, TrendlineType.Power, "Power Trendline");

            // Sparar Excel-filen
            workbook.Save("TrendlineTypeExample.xlsx");
        }

        private static void AddTrendline(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
        {
            // Lägga till en trendline av den angivna typen till den angivna serien
            int index = chart.NSeries[seriesIndex].TrendLines.Add(trendlineType);
            Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
            
            // Ställer in det anpassade namnet på trendlinjen
            trendline.Name = trendlineName;
            
            // Visar ekvationen i diagrammet
            trendline.DisplayEquation = true;
            
            // Visar R‑kvadratvärdet i diagrammet
            trendline.DisplayRSquared = true;
            
            // Ställ in färgen på trendline
            trendline.Color = Color.Red;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


