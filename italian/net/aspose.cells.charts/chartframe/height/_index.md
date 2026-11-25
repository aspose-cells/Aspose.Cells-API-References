---
title: "ChartFrame.Height"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta l'altezza del frame in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

Ottiene o imposta l'altezza del frame in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### Osservazioni

Come convertire le unità di 1/4000 in pixel? Altezza in pixel = Y * Chart.ChartObject.Height / 4000d;

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.HeightRatioToChart, invece. Altezza = HeightRatioToChart * 4000. Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyHeightDemo
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

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alle etichette dei dati
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Imposta la proprietà Height
            dataLabels.Height = 200; // Set height to 200 pixels
            
            // Visualizza il valore dell'altezza
            Console.WriteLine("DataLabels Height: " + dataLabels.Height);
            
            // Salva la cartella di lavoro
            workbook.Save("ChartFramePropertyHeightDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


