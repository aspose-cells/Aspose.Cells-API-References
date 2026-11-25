---
title: "ChartFrame.DefaultHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Rappresenta l'altezza della posizione predefinita in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/defaultheight/
---
## ChartFrame.DefaultHeight property

Rappresenta l'altezza della posizione predefinita in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use ChartFrame.DefaultHeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultHeight { get; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.DefaultHeightRatioToChart, invece. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultHeightDemo
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

            // Accedi al titolo del grafico (che è un ChartFrame)
            ChartFrame chartTitle = chart.Title;
            
            // Visualizza il valore corrente di DefaultHeight (proprietà di sola lettura)
            Console.WriteLine("Current DefaultHeight value: " + chartTitle.DefaultHeight);

            // Dimostra come DefaultHeight influisce sul layout del grafico
            Console.WriteLine("DefaultHeightRatioToChart: " + chartTitle.DefaultHeightRatioToChart);
            Console.WriteLine("Current HeightRatioToChart: " + chartTitle.HeightRatioToChart);

            // Regola l'altezza usando la proprietà scrivibile
            chartTitle.HeightRatioToChart = chartTitle.DefaultHeightRatioToChart * 1.5;
            Console.WriteLine("New HeightRatioToChart: " + chartTitle.HeightRatioToChart);

            // Salva il risultato
            workbook.Save("ChartFrameDefaultHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


