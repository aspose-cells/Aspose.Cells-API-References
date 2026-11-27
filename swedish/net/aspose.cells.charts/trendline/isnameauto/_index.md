---
title: "Trendline.IsNameAuto"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Trendline-egenskap. Returnerar om Microsoft Excel automatiskt bestämmer namnet på trendlinjen"
type: docs
url: /sv/net/aspose.cells.charts/trendline/isnameauto/
---
## Trendline.IsNameAuto property

Returnerar om Microsoft Excel automatiskt bestämmer namnet på trendlinjen.

```csharp
public bool IsNameAuto { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyIsNameAutoDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serie i diagrammet
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Lägg till trendlinje - modifierad för att säkerställa korrekt skapande av Trendline-objekt
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Demonstrera IsNameAuto-egenskapen
            Console.WriteLine("Initial IsNameAuto value: " + trendline.IsNameAuto);
            
            // Ange anpassat namn (inaktiverar automatisk namngivning)
            trendline.Name = "Custom Trendline Name";
            Console.WriteLine("After setting custom name, IsNameAuto: " + trendline.IsNameAuto);
            
            // Återställ till automatiskt namn
            trendline.IsNameAuto = true;
            Console.WriteLine("After setting IsNameAuto=true, Name: " + trendline.Name);
        }
    }
}
```

### Se även

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


