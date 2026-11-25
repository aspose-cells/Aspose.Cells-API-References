---
title: "Axis.CrossAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta il punto sull'asse dei valori dove l'asse delle categorie lo incrocia"
type: docs
url: /it/net/aspose.cells.charts/axis/crossat/
---
## Axis.CrossAt property

Rappresenta il punto sull'asse dei valori in cui l'asse delle categorie lo attraversa.

```csharp
public double CrossAt { get; set; }
```

### Osservazioni

Il numero deve essere un intero quando si applica all'asse delle categorie. Inoltre il valore deve essere compreso tra 1 e 31999.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCrossAtDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Configura l'asse dei valori
            chart.ValueAxis.CrossAt = 15; // Cross at value 15
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 50;

            // Configura l'asse delle categorie
            chart.CategoryAxis.CrossAt = 2.5; // Cross between categories B and C
            chart.CategoryAxis.TickLabelPosition = Aspose.Cells.Charts.TickLabelPositionType.Low;

            // Salva la cartella di lavoro
            workbook.Save("AxisCrossAtDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


