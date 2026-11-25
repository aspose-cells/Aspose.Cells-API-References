---
title: "Series.Shadow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. True se la serie ha un'ombra"
type: docs
url: /it/net/aspose.cells.charts/series/shadow/
---
## Series.Shadow property

Vero se la serie ha un'ombra.

```csharp
public bool Shadow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alla prima serie e abilita l'ombra
            Series series = chart.NSeries[0];
            series.Shadow = true;

            // Salva e ricarica per verificare
            workbook.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Series loadedSeries = loadedWorkbook.Worksheets[0].Charts[0].NSeries[0];
            Console.WriteLine("Shadow enabled: " + loadedSeries.Shadow);
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


