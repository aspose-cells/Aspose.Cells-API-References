---
title: "Trendline.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Trendline. Restituisce il tipo di trendline"
type: docs
url: /it/net/aspose.cells.charts/trendline/type/
---
## Trendline.Type property

Restituisce il tipo di linea di tendenza.

```csharp
public TrendlineType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["A5"].PutValue(4);
            
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["B3"].PutValue(4);
            sheet.Cells["B4"].PutValue(8);
            sheet.Cells["B5"].PutValue(16);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Aggiungi serie
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";

            // Aggiungi una trendline esponenziale
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Dimostra l'uso della proprietà Type
            Console.WriteLine("Trendline type: " + trendline.Type);
            
            // Salva la cartella di lavoro
            workbook.Save("TrendlinePropertyTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TrendlineType](../../trendlinetype/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


