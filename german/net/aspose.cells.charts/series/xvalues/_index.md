---
title: "Series.XValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Stellt die X‑Werte dieser Diagrammserie dar"
type: docs
url: /de/net/aspose.cells.charts/series/xvalues/
---
## Series.XValues property

Stellt die X‑Werte dieser Diagrammserie dar.

```csharp
public string XValues { get; set; }
```

### Hinweise

Nur für Scatter- und Bubble-Diagramme. Bitte verwenden Sie [`CategoryData`](../../seriescollection/categorydata/) für andere Diagrammtypen. [`CategoryValues`](../categoryvalues/) wird verwendet, um die tatsächlichen Kategorienwerte dieser Serie zu erhalten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            var workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i+1, 0].PutValue(i+1); // X values 1-5
                worksheet.Cells[i+1, 1].PutValue((i+1)*2); // Series 1 values
                worksheet.Cells[i+1, 2].PutValue((i+1)*3); // Series 2 values
            }

            // Ein Streudiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Serie mit XValues und Values hinzufügen
            int seriesIndex = chart.NSeries.Add("B2:B6", false);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property
            series.Name = "Series 1";

            seriesIndex = chart.NSeries.Add("C2:C6", false);
            series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property again
            series.Name = "Series 2";

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesXValuesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


