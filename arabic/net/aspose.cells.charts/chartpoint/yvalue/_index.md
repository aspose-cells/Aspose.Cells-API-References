---
title: "ChartPoint.YValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. يحصل على أو يضبط قيمة Y لنقطة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/yvalue/
---
## ChartPoint.YValue property

يحصل أو يعيّن قيمة Y لنقطة المخطط.

```csharp
public object YValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyYValueDemo
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
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // احصل على نقاط السلسلة الأولى
            Series series = chart.NSeries[0];
            var points = series.Points;

            // أظهر خاصية YValue
            Console.WriteLine("Y Values of Chart Points:");
            for (int i = 0; i < points.Count; i++)
            {
                Console.WriteLine($"Point {i + 1}: {points[i].YValue}");
            }

            // عدّل YValue لنقطة
            points[2].YValue = 50;
            Console.WriteLine($"\nModified Point 3 YValue to: {points[2].YValue}");

            // احفظ المصنف
            workbook.Save("ChartPointYValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


