---
title: "Legend.GetLegendLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Legend-metod. Hämtar etiketterna för legendposterna efter anrop av Chart.Calculate-metoden"
type: docs
url: /sv/net/aspose.cells.charts/legend/getlegendlabels/
---
## Legend.GetLegendLabels method

Hämtar etiketterna för förklaringsposterna efter att ha anropat metoden Chart.Calculate().

```csharp
public string[] GetLegendLabels()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendMethodGetLegendLabelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Beräkna diagrammet
            chart.Calculate();
            
            // Hämta legendetiketter
            string[] legendLabels = chart.Legend.GetLegendLabels();
            
            // Visa legendetiketter
            Console.WriteLine("Legend Labels:");
            foreach (string label in legendLabels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### Se även

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


