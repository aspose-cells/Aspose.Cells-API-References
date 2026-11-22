---
title: "ChartArea.Height"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartArea. تحصل أو تعين الإزاحة العمودية من صف الزاوية السفلية اليمنى بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartarea/height/
---
## ChartArea.Height property

تحصل أو تعين الإزاحة العمودية من صف الزاوية السفلية اليمنى، بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use ChartArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### ملاحظات

ملاحظة: هذه العضوية أصبحت الآن مهجورة. يرجى استخدام خاصية ChartArea.HeightRatioToChart بدلاً من ذلك. الارتفاع = HeightRatioToChart * 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyHeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى مساحة المخطط
            ChartArea chartArea = chart.ChartArea;

            // عرض خاصية Height
            Console.WriteLine("Original Chart Area Height: " + chartArea.Height);
            
            // تعديل الارتفاع
            chartArea.Height = 500;
            Console.WriteLine("Modified Chart Area Height: " + chartArea.Height);

            // احفظ المصنف
            workbook.Save("ChartAreaHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


