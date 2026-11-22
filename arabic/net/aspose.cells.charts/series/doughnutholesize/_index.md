---
title: "Series.DoughnutHoleSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية السلسلة. تُرجع أو تُعيّن حجم الفتحة في مجموعة مخطط الدونات. يُعبّر عن حجم الفتحة كنسبة مئوية من حجم المخطط بين 10 و 90 بالمئة"
type: docs
url: /ar/net/aspose.cells.charts/series/doughnutholesize/
---
## Series.DoughnutHoleSize property

يعيد أو يضبط حجم الفتحة في مجموعة مخطط الدونات. يُعبّر عن حجم الفتحة كنسبة مئوية من حجم المخطط، بين 10 و90 بالمائة.

```csharp
public int DoughnutHoleSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDoughnutHoleSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // أضف مخطط Doughnut
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين حجم فتحة الدونات (نسبة مئوية من نصف قطر المخطط)
            chart.NSeries[0].DoughnutHoleSize = 25;

            // احفظ المصنف
            workbook.Save("DoughnutHoleSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


