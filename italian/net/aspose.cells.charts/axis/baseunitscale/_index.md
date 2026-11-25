---
title: "Axis.BaseUnitScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà dell'asse. Rappresenta la scala dell'unità base per l'asse delle categorie"
type: docs
url: /it/net/aspose.cells.charts/axis/baseunitscale/
---
## Axis.BaseUnitScale property

Rappresenta la scala dell'unità di base per l'asse delle categorie.

```csharp
public TimeUnit BaseUnitScale { get; set; }
```

### Osservazioni

Ha effetto solo quando la proprietà CategoryType è impostata su TimeScale.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBaseUnitScaleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddDays(i));
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Imposta la scala dell'unità base per l'asse delle categorie
            chart.CategoryAxis.BaseUnitScale = TimeUnit.Months;

            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyBaseUnitScaleDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


