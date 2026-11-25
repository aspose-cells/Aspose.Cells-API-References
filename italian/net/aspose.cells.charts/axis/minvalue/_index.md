---
title: "Axis.MinValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta il valore minimo sull'asse dei valori"
type: docs
url: /it/net/aspose.cells.charts/axis/minvalue/
---
## Axis.MinValue property

Rappresenta il valore minimo sull'asse dei valori.

```csharp
public object MinValue { get; set; }
```

### Osservazioni

Il tipo minValue può essere solo double o DateTime

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(40);
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(60);

            // Aggiungi un grafico e imposta l'intervallo dei dati
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", false);

            // Configura le proprietà dell'asse dei valori
            chart.ValueAxis.MinValue = 15;  // Setting minimum value
            chart.ValueAxis.MaxValue = 70;
            chart.ValueAxis.MajorUnit = 10;

            // Salva la cartella di lavoro
            workbook.Save("AxisMinValueDemo.xlsx");

            Console.WriteLine("Chart created with MinValue set to 15.");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


