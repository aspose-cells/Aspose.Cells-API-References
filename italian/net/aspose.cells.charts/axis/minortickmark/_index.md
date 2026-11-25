---
title: "Axis.MinorTickMark"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta il tipo di segno di graduazione minore per l'asse specificato"
type: docs
url: /it/net/aspose.cells.charts/axis/minortickmark/
---
## Axis.MinorTickMark property

Rappresenta il tipo di segnapunto secondario per l'asse specificato.

```csharp
public TickMarkType MinorTickMark { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorTickMarkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configura le proprietà dell'asse
            Axis valueAxis = chart.ValueAxis;
            valueAxis.MinorTickMark = TickMarkType.Inside;
            valueAxis.MajorTickMark = TickMarkType.Cross;
            valueAxis.MinValue = 0;
            valueAxis.MaxValue = 200;
            valueAxis.MajorUnit = 25;

            workbook.Save("AxisMinorTickMarkDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


