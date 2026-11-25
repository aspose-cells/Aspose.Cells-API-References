---
title: "ChartPoint.ArcEndPointYPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la coordinata y del punto finale per la sezione a torta dopo le chiamate al metodo Chart.Calculate. Si applica ai grafici a torta e ciambella"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/arcendpointypx/
---
## ChartPoint.ArcEndPointYPx property

Ottiene la coordinata y del punto finale per la sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici a torta e ciambella.

```csharp
public float ArcEndPointYPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(12000);
            worksheet.Cells["B4"].PutValue(14000);

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per ottenere le posizioni delle forme
            chart.Calculate();

            // Ottieni il primo punto del grafico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore corrente di ArcEndPointYPx
            Console.WriteLine("Current ArcEndPointYPx value: " + point.ArcEndPointYPx);

            // Poiché ArcEndPointYPx è di sola lettura, possiamo solo leggerlo
            // La riga seguente causerebbe un errore di compilazione:
            // point.ArcEndPointYPx = 150.5f;

            // Dimostra come questa proprietà influisce sul grafico a torta
            Console.WriteLine("Pie slice end point Y coordinate: " + point.ArcEndPointYPx + " pixels");

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


