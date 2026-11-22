---
title: "Series.BubbleScale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. يحصل أو يضبط عامل المقياس للفقاعات في مجموعة المخطط المحددة. يمكن أن يكون قيمة صحيحة من 0 إلى 300 تمثل نسبة مئوية من الحجم الافتراضي. ينطبق فقط على المخططات الفقاعية"
type: docs
url: /ar/net/aspose.cells.charts/series/bubblescale/
---
## Series.BubbleScale property

يحصل أو يحدد عامل المقياس للفقاعات في مجموعة المخطط المحددة. يمكن أن يكون قيمة صحيحة من 0 (صفر) إلى 300، تمثل نسبة مئوية من الحجم الافتراضي. ينطبق فقط على مخططات الفقاعات.

```csharp
public int BubbleScale { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleScaleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لمخطط الفقاعات
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["C1"].PutValue("Size");
            
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(5);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["C3"].PutValue(10);
            
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C4"].PutValue(15);

            // إضافة مخطط فقاعات
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة إلى المخطط
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries[seriesIndex].XValues = "A2:A4";
            chart.NSeries[seriesIndex].BubbleSizes = "C2:C4";
            
            // تعيين مقياس الفقاعات لتوضيح الخاصية
            chart.NSeries[seriesIndex].BubbleScale = 150; // Scale bubbles to 150% of default size
            
            // تخصيص مظهر المخطط
            chart.Title.Text = "Bubble Chart with Scaled Bubbles";
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.LightBlue, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
            
            // احفظ المصنف
            workbook.Save("BubbleScaleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


