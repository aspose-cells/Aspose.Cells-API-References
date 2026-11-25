---
title: "Chart.IsChartDataChanged"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Rileva se la sorgente dati del grafico è cambiata"
type: docs
url: /it/net/aspose.cells.charts/chart/ischartdatachanged/
---
## Chart.IsChartDataChanged method

Rileva se la sorgente dati di un grafico è cambiata.

```csharp
public bool IsChartDataChanged()
```

### Valore di ritorno

Restituisce true se il grafico è cambiato, altrimenti restituisce false

### Osservazioni

Il metodo rileva le modifiche nella sorgente dati del grafico prima di renderizzare il grafico in formato immagine. Alla prima chiamata a Chart.toImage, i dati di origine del grafico (ad es. XValuesParseData, ValuesParseData) verranno registrati. Prima di chiamare nuovamente il metodo Chart.toImage, chiamare il metodo IsChartDataChanged per verificare se il grafico necessita di un nuovo rendering.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsChartDataChangedDemo
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

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Verifica se i dati del grafico sono cambiati (dovrebbe essere false inizialmente)
                bool isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after creation: {isChanged}");

                // Modifica i dati del grafico
                worksheet.Cells["B2"].PutValue(15);

                // Verifica nuovamente se i dati del grafico sono cambiati
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after modification: {isChanged}");

                // Calcola il grafico per aggiornarlo
                chart.Calculate();

                // Verifica dopo il calcolo
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after calculation: {isChanged}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsChartDataChanged method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("ChartMethodIsChartDataChangedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


