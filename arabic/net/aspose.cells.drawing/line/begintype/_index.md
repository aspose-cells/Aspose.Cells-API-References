---
title: "Line.BeginType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Line. تحدد رأس سهم لبداية الخط"
type: docs
url: /ar/net/aspose.cells.drawing/line/begintype/
---
## Line.BeginType property

يحدد رأس السهم لبداية الخط.

```csharp
public MsoArrowheadStyle BeginType { get; set; }
```

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // إضافة مخطط خطي
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("A1:A3", true);

            // احصل على السلسلة الأولى وقم بتكوين خصائص الخط الخاصة بها
            Series series = chart.NSeries[0];
            series.Border.BeginType = MsoArrowheadStyle.Arrow;
            series.Border.EndType = MsoArrowheadStyle.ArrowDiamond;
            series.Border.Color = Color.Red;
            series.Border.Weight = WeightType.MediumLine;

            // احفظ المصنف
            workbook.Save("LinePropertyBeginTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


