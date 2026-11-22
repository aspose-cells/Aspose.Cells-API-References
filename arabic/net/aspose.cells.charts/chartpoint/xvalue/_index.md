---
title: "ChartPoint.XValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. يحصل على أو يحدد قيمة X لنقطة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/xvalue/
---
## ChartPoint.XValue property

يحصل أو يعيّن قيمة X لنقطة المخطط.

```csharp
public object XValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyXValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(50);
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // تخصيص نقاط البيانات
            for (int i = 0; i < chart.NSeries[0].Points.Count; i++)
            {
                ChartPoint point = chart.NSeries[0].Points[i];
                
                // عرض استخدام خاصية XValue
                point.XValue = "Modified " + (i + 1);
                
                // تنسيق إضافي لتحسين الرؤية
                point.Area.ForegroundColor = Color.FromArgb(100 + i * 50, 150, 200);
            }

            workbook.Save("ChartPointXValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


