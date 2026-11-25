---
title: "ChartFrame.DefaultWidthRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Rappresenta la larghezza della posizione predefinita in unità di frazione dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/defaultwidthratiotochart/
---
## ChartFrame.DefaultWidthRatioToChart property

Rappresenta la larghezza della posizione predefinita in unità di frazione dell'area del grafico.

```csharp
public double DefaultWidthRatioToChart { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthRatioToChartDemo
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

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi al titolo del grafico che è un ChartFrame
            ChartFrame chartTitle = chart.Title;

            // Visualizza il valore corrente di DefaultWidthRatioToChart
            Console.WriteLine("Current DefaultWidthRatioToChart value: " + chartTitle.DefaultWidthRatioToChart);

            // Nota: DefaultWidthRatioToChart è di sola lettura, quindi non possiamo impostarlo
            // Invece, dimostreremo la sua relazione con il rapporto di larghezza reale
            Console.WriteLine("Current WidthRatioToChart: " + chartTitle.WidthRatioToChart);

            // Modifica il rapporto di larghezza per dimostrarne l'effetto
            chartTitle.WidthRatioToChart = 0.5;
            Console.WriteLine("After setting WidthRatioToChart to 0.5, DefaultWidthRatioToChart remains: " + chartTitle.DefaultWidthRatioToChart);

            // Salva la cartella di lavoro
            workbook.Save("ChartFramePropertyDefaultWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


