---
title: "Chart.IsReferedByChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Restituisce se la cella è riferita dal grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/isreferedbychart/
---
## Chart.IsReferedByChart method

Restituisce se la cella è riferita dal grafico.

```csharp
[Obsolete("Use Chart.IsCellReferedByChart(int,int,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsReferedByChart(int rowIndex, int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | L'indice della riga |
| columnIndex | Int32 | L'indice di colonna |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo IsCellReferedByChart(int,int,int). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2023. Aspose si scusa per eventuali inconvenienti che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsReferedByChartWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Verifica se la cella B2 (riga 1, colonna 1) è riferita dal grafico
                bool isReferred = chart.IsReferedByChart(1, 1);
                
                Console.WriteLine($"Is cell B2 referred by the chart? {isReferred}");
                
                // Verifica una cella che non è nell'intervallo dei dati del grafico
                bool isNotReferred = chart.IsReferedByChart(10, 10);
                Console.WriteLine($"Is cell K11 referred by the chart? {isNotReferred}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsReferedByChart method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ChartMethodIsReferedByChartWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


