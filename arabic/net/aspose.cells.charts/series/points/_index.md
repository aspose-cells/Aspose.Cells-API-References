---
title: "Series.Points"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تحصل على مجموعة النقاط في سلسلة داخل مخطط"
type: docs
url: /ar/net/aspose.cells.charts/series/points/
---
## Series.Points property

يحصل على مجموعة النقاط في سلسلة داخل مخطط.

```csharp
public ChartPointCollection Points { get; }
```

### ملاحظات

عند كون المخطط Pie of Pie أو Bar of Pie، تكون النقطة الأخيرة نقطة أخرى في مخطط الفطيرة الأول

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPointsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى السلسلة الأولى ونقاطها
            Series series = chart.NSeries[0];
            foreach (ChartPoint point in series.Points)
            {
                // أضف تسميات البيانات إلى كل نقطة
                point.DataLabels.ShowValue = true;
                point.DataLabels.ShowCellRange = true;
            }

            // احفظ المصنف
            workbook.Save("SeriesPropertyPointsDemo_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


