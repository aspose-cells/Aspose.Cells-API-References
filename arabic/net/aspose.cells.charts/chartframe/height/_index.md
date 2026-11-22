---
title: "ChartFrame.Height"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. يحصل أو يضبط ارتفاع الإطار بوحدات 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

يحصل أو يضبط ارتفاع الإطار بوحدات 1/4000 من مساحة المخطط.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### ملاحظات

كيف يتم تحويل الوحدات 1/4000 إلى بكسل؟ الارتفاع بالبكسل = Y * Chart.ChartObject.Height / 4000d;

ملاحظة: هذا العضو أصبح الآن غير صالح. يرجى استخدام خاصية ChartFrame.HeightRatioToChart بدلاً من ذلك. الارتفاع = HeightRatioToChart * 4000. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyHeightDemo
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
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى تسميات البيانات
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // ضبط خاصية Height
            dataLabels.Height = 200; // Set height to 200 pixels
            
            // عرض قيمة الارتفاع
            Console.WriteLine("DataLabels Height: " + dataLabels.Height);
            
            // احفظ المصنف
            workbook.Save("ChartFramePropertyHeightDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


