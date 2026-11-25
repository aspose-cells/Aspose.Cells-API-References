---
title: "ChartPoint.StartAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene l'angolo di partenza per la sezione a torta misurato in gradi in senso orario dall'asse x dopo aver chiamato il metodo Chart.Calculate. Si applica al grafico a torta"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/startangle/
---
## ChartPoint.StartAngle property

Ottiene l'angolo di partenza per la sezione della pie, misurato in gradi in senso orario dall'asse x dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico Pie.

```csharp
public float StartAngle { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyStartAngleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

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

            // Visualizza il valore StartAngle
            Console.WriteLine("StartAngle of first pie slice: " + point.StartAngle);

            // Nota: StartAngle è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare l'angolo di partenza, è necessario ruotare l'intero grafico a torta
            chart.NSeries[0].FirstSliceAngle = 90; // Rotate pie chart by 90 degrees

            // Ricalcola per aggiornare gli angoli
            chart.Calculate();

            // Visualizza il nuovo valore StartAngle dopo la rotazione
            Console.WriteLine("StartAngle after rotation: " + point.StartAngle);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyStartAngleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


