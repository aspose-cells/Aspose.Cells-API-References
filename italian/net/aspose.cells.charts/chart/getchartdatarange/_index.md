---
title: "Chart.GetChartDataRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Ottiene l'intervallo dell'origine dati del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/getchartdatarange/
---
## Chart.GetChartDataRange method

Ottiene l'intervallo della sorgente dati del grafico.

```csharp
public string GetChartDataRange()
```

### Valore di ritorno

L'origine dati.

### Osservazioni

Supporta solo gli intervalli. Se Series.Values, Name e XValues sono in un intervallo continuo, verrà restituito un intervallo che li contiene.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodGetChartDataRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C4"].PutValue(60);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("=Sheet1!$B$1:$C$4", true);
            
            // Ottieni e visualizza l'intervallo dei dati del grafico
            string dataRange = chart.GetChartDataRange();
            Console.WriteLine("Chart Data Range: " + dataRange);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


