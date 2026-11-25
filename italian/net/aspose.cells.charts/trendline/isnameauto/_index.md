---
title: "Trendline.IsNameAuto"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Trendline. Restituisce se Microsoft Excel determina automaticamente il nome della trendline"
type: docs
url: /it/net/aspose.cells.charts/trendline/isnameauto/
---
## Trendline.IsNameAuto property

Restituisce se Microsoft Excel determina automaticamente il nome della linea di tendenza.

```csharp
public bool IsNameAuto { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie al grafico
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Aggiungi trendline - modificato per garantire la corretta creazione dell'oggetto Trendline
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Dimostra la proprietà IsNameAuto
            Console.WriteLine("Initial IsNameAuto value: " + trendline.IsNameAuto);
            
            // Imposta nome personalizzato (disabilita la denominazione automatica)
            trendline.Name = "Custom Trendline Name";
            Console.WriteLine("After setting custom name, IsNameAuto: " + trendline.IsNameAuto);
            
            // Ripristina al nome automatico
            trendline.IsNameAuto = true;
            Console.WriteLine("After setting IsNameAuto=true, Name: " + trendline.Name);
        }
    }
}
```

### Vedi anche

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


