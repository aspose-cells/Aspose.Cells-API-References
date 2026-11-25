---
title: "Axis.IsDisplayUnitLabelShown"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Indica se l'etichetta dell'unità di visualizzazione è mostrata sull'asse specificato"
type: docs
url: /it/net/aspose.cells.charts/axis/isdisplayunitlabelshown/
---
## Axis.IsDisplayUnitLabelShown property

Rappresenta se l'etichetta dell'unità di visualizzazione è mostrata sull'asse specificato.

```csharp
public bool IsDisplayUnitLabelShown { get; set; }
```

### Osservazioni

Il valore predefinito è True. Funziona solo quando [`DisplayUnit`](../displayunit/) non è None.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsDisplayUnitLabelShownDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dati di esempio
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            
            // Configura la visibilità dell'unità di visualizzazione e dell'etichetta
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            workbook.Save("AxisPropertyIsDisplayUnitLabelShownDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


