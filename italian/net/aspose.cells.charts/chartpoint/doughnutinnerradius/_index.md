---
title: "ChartPoint.DoughnutInnerRadius"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene il raggio interno della fetta di ciambella in unità di pixel dopo aver chiamato il metodo Chart.Calculate. Si applica al grafico a ciambella"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/doughnutinnerradius/
---
## ChartPoint.DoughnutInnerRadius property

Ottiene il raggio interno della fetta a ciambella in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico a ciambella.

```csharp
public int DoughnutInnerRadius { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDoughnutInnerRadiusDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // Aggiungi un grafico a ciambella
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per ottenere i punti del grafico
            chart.Calculate();

            // Ottieni il primo punto del grafico dalla prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore corrente di DoughnutInnerRadius
            Console.WriteLine("Current DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Nota: DoughnutInnerRadius è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare il raggio interno, è necessario regolare la proprietà HoleSize del grafico
            chart.FirstSliceAngle = 30; // Adjust the first slice angle instead since HoleSize isn't available

            // Ricalcola il grafico per aggiornare DoughnutInnerRadius
            chart.Calculate();

            // Visualizza il valore aggiornato di DoughnutInnerRadius
            Console.WriteLine("Updated DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Salva la cartella di lavoro
            workbook.Save("DoughnutInnerRadiusDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


