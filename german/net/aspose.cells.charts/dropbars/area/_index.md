---
title: "DropBars.Area"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DropBars-Eigenschaft. Gibt den Area zurück"
type: docs
url: /de/net/aspose.cells.charts/dropbars/area/
---
## DropBars.Area property

Gibt den `Area` zurück.

```csharp
public Area Area { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DropBarsPropertyAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            chart.NSeries.Add("A1:B3", true);
            chart.NSeries[0].HasUpDownBars = true;

            Aspose.Cells.Charts.DropBars upBars = chart.NSeries[0].UpBars;
            Aspose.Cells.Charts.DropBars downBars = chart.NSeries[0].DownBars;

            upBars.Area.ForegroundColor = Color.LightGreen;
            upBars.Area.FillFormat.SetOneColorGradient(Color.LightGreen, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
            
            downBars.Area.ForegroundColor = Color.LightCoral;
            downBars.Area.FillFormat.SetOneColorGradient(Color.LightCoral, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);

            workbook.Save("DropBarsPropertyAreaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Area](../../../aspose.cells.drawing/area/)
* class [DropBars](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


