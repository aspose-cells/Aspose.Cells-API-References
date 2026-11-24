---
title: "Series.BubbleSizes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt die Bubble‑Größenwerte der Diagrammserie zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.charts/series/bubblesizes/
---
## Series.BubbleSizes property

Liest oder legt die Blasengrößenwerte der Diagrammreihe fest.

```csharp
public string BubbleSizes { get; set; }
```

### Hinweise

Nur für Bubble oder Bubble3D.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleSizesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Blasendiagramm hinzufügen
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["C1"].PutValue("Bubble Sizes");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
                worksheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Ein Blasendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Bubble, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Setze Seriendaten mittels der BubbleSizes‑Eigenschaft
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";
            chart.NSeries[0].BubbleSizes = "C2:C5";

            // Speichere die Arbeitsmappe
            workbook.Save("BubbleChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


