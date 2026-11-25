---
title: "ChartPoint.RadiusPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene il raggio della torta a bolle o ciambella in unità di pixel dopo le chiamate al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/radiuspx/
---
## ChartPoint.RadiusPx property

Ottiene il raggio di bubble, pie o doughnut in unità di pixel dopo le chiamate al metodo Chart.Calculate().

```csharp
public int RadiusPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyRadiusPxDemo
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

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che le proprietà siano popolate
            chart.Calculate();

            // Ottieni il primo punto del grafico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore corrente del raggio
            Console.WriteLine("Current RadiusPx value: " + point.RadiusPx);

            // Nota: RadiusPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare il raggio, dobbiamo regolare le dimensioni del grafico o altre proprietà
            // che influenzano la dimensione del punto indirettamente

            // Esempio di come la modifica delle dimensioni del grafico influisce sul raggio
            Console.WriteLine("\nChanging chart size to demonstrate radius change...");
            chart.ChartObject.Width = 800;
            chart.ChartObject.Height = 600;
            chart.Calculate();

            // Visualizza il nuovo valore del raggio dopo il ridimensionamento del grafico
            Console.WriteLine("New RadiusPx value after chart resize: " + point.RadiusPx);

            // Salva il risultato
            workbook.Save("ChartPointPropertyRadiusPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


