---
title: "Line.EndArrowWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخط. تحدد عرض رأس السهم لنهاية الخط"
type: docs
url: /ar/net/aspose.cells.drawing/line/endarrowwidth/
---
## Line.EndArrowWidth property

يحدد عرض رأس السهم لنهاية الخط.

```csharp
public MsoArrowheadWidth EndArrowWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LinePropertyEndArrowWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لمخطط الخط
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // إضافة مخطط خطي
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("A1:B3", true);

            // تكوين خصائص الخط للسلسلة الأولى
            Series series = chart.NSeries[0];
            series.Border.EndArrowWidth = MsoArrowheadWidth.Wide;
            series.Border.EndType = MsoArrowheadStyle.Arrow;

            // احفظ المصنف
            workbook.Save("LinePropertyEndArrowWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


