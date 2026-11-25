---
title: "Axis.TickLabelPosition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta la posizione delle etichette dei segni di graduazione sull'asse specificato"
type: docs
url: /it/net/aspose.cells.charts/axis/ticklabelposition/
---
## Axis.TickLabelPosition property

Rappresenta la posizione delle etichette dei segni di graduazione sull'asse specificato.

```csharp
public TickLabelPositionType TickLabelPosition { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelPositionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Imposta la posizione dell'etichetta del segno di graduazione
            chart.CategoryAxis.TickLabelPosition = TickLabelPositionType.Low;
            
            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyTickLabelPositionDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TickLabelPositionType](../../ticklabelpositiontype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


