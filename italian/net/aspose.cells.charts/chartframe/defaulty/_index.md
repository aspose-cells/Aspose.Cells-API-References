---
title: "ChartFrame.DefaultY"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Rappresenta il valore y della posizione predefinita in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/defaulty/
---
## ChartFrame.DefaultY property

Rappresenta il valore y della posizione predefinita in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use ChartFrame.DefaultYRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultY { get; }
```

### Osservazioni

NOTA: questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.DefaultYRatioToChart, invece. DefaultY = (int)(DefaultYRatioToChart * 4000); Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYDemo
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
            
            // Accedi al titolo del grafico che eredita da ChartFrame
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;
            
            // Visualizza il valore corrente di DefaultY (proprietà di sola lettura)
            Console.WriteLine("DefaultY value (1/4000 of chart area): " + chartFrame.DefaultY);
            Console.WriteLine("DefaultY ratio to chart area: " + chartFrame.DefaultYRatioToChart);
            
            // Dimostra come DefaultY influisce sul posizionamento confrontandolo con la posizione corrente
            Console.WriteLine("Current Y position (ratio): " + chartFrame.YRatioToChart);
            
            // Ripristina la posizione predefinita usando SetPositionAuto()
            chartFrame.SetPositionAuto();
            Console.WriteLine("Y position after reset (ratio): " + chartFrame.YRatioToChart);
            
            // Salva il risultato
            workbook.Save("ChartFramePropertyDefaultYDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


