---
title: "Line.EndType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخط. تحدد رأس السهم لنهاية الخط"
type: docs
url: /ar/net/aspose.cells.drawing/line/endtype/
---
## Line.EndType property

يحدد رأس السهم لنهاية الخط.

```csharp
public MsoArrowheadStyle EndType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyEndTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // إضافة خط اتجاه وضبط EndType
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.EndType = MsoArrowheadStyle.Arrow;
            trendline.EndArrowLength = MsoArrowheadLength.Medium;
            trendline.EndArrowWidth = MsoArrowheadWidth.Medium;

            workbook.Save("LineEndTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


