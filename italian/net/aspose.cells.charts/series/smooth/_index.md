---
title: "Series.Smooth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà della serie. Rappresenta l'ammorbidimento della curva. True se l'ammorbidimento della curva è attivato per il grafico a linee o a dispersione. Si applica solo ai grafici a linee e ai grafici a dispersione con linee"
type: docs
url: /it/net/aspose.cells.charts/series/smooth/
---
## Series.Smooth property

Rappresenta l'ammorbidimento della curva. Vero se l'ammorbidimento della curva è attivato per il grafico a linee o a dispersione. Si applica solo ai grafici a linee e ai grafici a dispersione con linee.

```csharp
public bool Smooth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySmoothDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta la proprietà Smooth per la prima serie
            chart.NSeries[0].Smooth = true;

            // Salva la cartella di lavoro
            workbook.Save("SmoothPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


