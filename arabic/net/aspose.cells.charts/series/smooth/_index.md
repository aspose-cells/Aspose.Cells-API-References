---
title: "Series.Smooth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية السلسلة. تمثل تنعيم المنحنى. صحيحة إذا تم تشغيل تنعيم المنحنى لمخطط الخط أو مخطط التشتت. ينطبق فقط على مخططات الخط ومخططات التشتت ذات الخطوط"
type: docs
url: /ar/net/aspose.cells.charts/series/smooth/
---
## Series.Smooth property

يمثل تنعيم المنحنى. صحيح إذا تم تشغيل تنعيم المنحنى لمخطط الخط أو مخطط التشتت. ينطبق فقط على مخططات الخط ومخططات التشتت ذات الخطوط.

```csharp
public bool Smooth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySmoothDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين خاصية Smooth للسلسلة الأولى
            chart.NSeries[0].Smooth = true;

            // احفظ المصنف
            workbook.Save("SmoothPropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


