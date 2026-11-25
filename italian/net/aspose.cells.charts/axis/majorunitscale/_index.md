---
title: "Axis.MajorUnitScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta la scala dell'unità principale per l'asse delle categorie"
type: docs
url: /it/net/aspose.cells.charts/axis/majorunitscale/
---
## Axis.MajorUnitScale property

Rappresenta la scala dell'unità principale per l'asse delle categorie.

```csharp
public TimeUnit MajorUnitScale { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio a scala temporale
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 5, 1));
            worksheet.Cells["B4"].PutValue(30);
            
            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);
            
            // Configura l'asse delle categorie come scala temporale con unità principale ogni 2 mesi
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;
            
            workbook.Save("AxisPropertyMajorUnitScaleDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


