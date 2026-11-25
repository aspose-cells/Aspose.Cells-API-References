---
title: "ChartFrame.DefaultXRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Rappresenta x della posizione predefinita in unità di frazione dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/defaultxratiotochart/
---
## ChartFrame.DefaultXRatioToChart property

Rappresenta x della posizione predefinita in unità di frazione dell'area del grafico.

```csharp
public double DefaultXRatioToChart { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni il frame del titolo del grafico
            ChartFrame titleFrame = chart.Title;

            // Visualizza il valore corrente di DefaultXRatioToChart
            Console.WriteLine("Default X Ratio To Chart (Title): " + titleFrame.DefaultXRatioToChart);

            // Crea una casella di testo nel grafico
            Aspose.Cells.Drawing.TextBox textBox = chart.Shapes.AddTextBoxInChart(50, 50, 200, 100);
            
            // Ottieni le proprietà della forma della casella di testo invece di provare ad accedere direttamente a ChartFrame
            Console.WriteLine("Default X Ratio To Chart (TextBox): " + titleFrame.DefaultXRatioToChart);

            // Dimostra come questi rapporti predefiniti influenzano il posizionamento
            Console.WriteLine("Title X Position (Ratio): " + titleFrame.XRatioToChart);
            Console.WriteLine("TextBox X Position (Ratio): " + titleFrame.XRatioToChart);

            // Salva la cartella di lavoro
            workbook.Save("ChartFrameDefaultXRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


