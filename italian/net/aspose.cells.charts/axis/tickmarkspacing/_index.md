---
title: "Axis.TickMarkSpacing"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Restituisce o imposta il numero di categorie o serie tra i ticchetti. Si applica solo agli assi di categoria e di serie"
type: docs
url: /it/net/aspose.cells.charts/axis/tickmarkspacing/
---
## Axis.TickMarkSpacing property

Restituisce o imposta il numero di categorie o serie tra i segni di graduazione. Si applica solo agli assi di categoria e di serie.

```csharp
public int TickMarkSpacing { get; set; }
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
    public class AxisPropertyTickMarkSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configura l'asse dei valori con TickMarkSpacing
            Axis valueAxis = chart.ValueAxis;
            valueAxis.MinValue = 0;
            valueAxis.MaxValue = 200;
            valueAxis.MajorUnit = 25;
            valueAxis.MinorUnit = 5;
            valueAxis.TickMarkSpacing = 2; // Setting tick mark spacing
            
            // Configura l'asse di categoria con TickMarkSpacing
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.TickMarkSpacing = 1; // Setting tick mark spacing

            workbook.Save("AxisTickMarkSpacingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


