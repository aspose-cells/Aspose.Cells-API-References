---
title: "Axis.MinorUnitScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta la scala dell'unità principale per l'asse delle categorie"
type: docs
url: /it/net/aspose.cells.charts/axis/minorunitscale/
---
## Axis.MinorUnitScale property

Rappresenta la scala dell'unità principale per l'asse delle categorie.

```csharp
public TimeUnit MinorUnitScale { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorUnitScaleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio basati sul tempo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddMonths(i - 2));
                worksheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Configura l'asse delle categorie come scala temporale
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyMinorUnitScaleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


