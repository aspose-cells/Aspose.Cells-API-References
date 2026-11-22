---
title: "SeriesCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SeriesCollection. تحصل على عنصر Series عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/item/
---
## SeriesCollection indexer

يحصل على عنصر [`Series`](../../series/) عند الفهرس المحدد.

```csharp
public Series this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Series");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Values");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى السلسلة الأولى والنقطة الأولى لها باستخدام خاصية Item
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            // تخصيص مظهر النقطة
            point.Area.FillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.White, GradientStyleType.Vertical, 2);
            point.Area.FillFormat.FillType = FillType.Solid;

            // احفظ المصنف
            workbook.Save("SeriesCollectionPropertyItemDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


