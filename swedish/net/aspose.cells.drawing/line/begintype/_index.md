---
title: "Line.BeginType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Linjeegenskap. Anger en pilspets för början av en linje"
type: docs
url: /sv/net/aspose.cells.drawing/line/begintype/
---
## Line.BeginType property

Anger en pilspets för början av en linje.

```csharp
public MsoArrowheadStyle BeginType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Lägg till ett linjediagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("A1:A3", true);

            // Hämta den första serien och konfigurera dess linjeegenskaper
            Series series = chart.NSeries[0];
            series.Border.BeginType = MsoArrowheadStyle.Arrow;
            series.Border.EndType = MsoArrowheadStyle.ArrowDiamond;
            series.Border.Color = Color.Red;
            series.Border.Weight = WeightType.MediumLine;

            // Spara arbetsboken
            workbook.Save("LinePropertyBeginTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


