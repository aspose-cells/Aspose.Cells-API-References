---
title: "Line.BeginArrowWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Specifica la larghezza della punta di freccia per l'inizio di una linea"
type: docs
url: /it/net/aspose.cells.drawing/line/beginarrowwidth/
---
## Line.BeginArrowWidth property

Specifica la larghezza della punta della freccia per l'inizio di una linea.

```csharp
public MsoArrowheadWidth BeginArrowWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginArrowWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Aggiungi una linea di tendenza e imposta le proprietà della freccia
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.BeginType = MsoArrowheadStyle.Arrow;
            trendline.BeginArrowWidth = MsoArrowheadWidth.Wide;
            trendline.EndType = MsoArrowheadStyle.Arrow;
            trendline.EndArrowWidth = MsoArrowheadWidth.Narrow;

            workbook.Save("LinePropertyBeginArrowWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


