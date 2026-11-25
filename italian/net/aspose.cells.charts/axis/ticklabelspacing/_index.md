---
title: "Axis.TickLabelSpacing"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta il numero di categorie o serie tra le etichette dei segni di graduazione. Si applica solo agli assi delle categorie e delle serie"
type: docs
url: /it/net/aspose.cells.charts/axis/ticklabelspacing/
---
## Axis.TickLabelSpacing property

Rappresenta il numero di categorie o serie tra le etichette dei segni di graduazione. Si applica solo agli assi di categoria e di serie.

```csharp
public int TickLabelSpacing { get; set; }
```

### Osservazioni

Il numero deve essere compreso tra 1 e 31999.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta i dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Configura la spaziatura delle etichette dei segni di graduazione dell'asse
            chart.CategoryAxis.TickLabelSpacing = 2; // Show every 2nd label

            workbook.Save("AxisPropertyTickLabelSpacingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


