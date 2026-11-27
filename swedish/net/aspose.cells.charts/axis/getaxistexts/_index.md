---
title: "Axis.GetAxisTexts"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-metod. Hämtar axelns etiketter efter anrop av metoden Chart.Calculate"
type: docs
url: /sv/net/aspose.cells.charts/axis/getaxistexts/
---
## Axis.GetAxisTexts method

Hämtar axelns etiketter efter anrop av metoden Chart.Calculate().

```csharp
public string[] GetAxisTexts()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisMethodGetAxisTextsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(4000);
            worksheet.Cells["B4"].PutValue(-8000);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Beräkna diagrammet
            chart.Calculate();
            
            // Hämta axelns etiketter
            string[] labels = chart.ValueAxis.GetAxisTexts();
            
            // Skriv ut etiketterna
            Console.WriteLine("Value Axis Labels:");
            foreach (string label in labels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


