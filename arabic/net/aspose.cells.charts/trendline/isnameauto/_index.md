---
title: "Trendline.IsNameAuto"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Trendline. تُعيد ما إذا كان Microsoft Excel يحدد اسم خط الاتجاه تلقائيًا"
type: docs
url: /ar/net/aspose.cells.charts/trendline/isnameauto/
---
## Trendline.IsNameAuto property

يعيد ما إذا كان Microsoft Excel يحدد اسم خط الاتجاه تلقائيًا.

```csharp
public bool IsNameAuto { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyIsNameAutoDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة إلى المخطط
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // إضافة خط اتجاه - تم تعديلها لضمان إنشاء كائن Trendline بشكل صحيح
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // عرض خاصية IsNameAuto
            Console.WriteLine("Initial IsNameAuto value: " + trendline.IsNameAuto);
            
            // تعيين اسم مخصص (يعطل التسمية التلقائية)
            trendline.Name = "Custom Trendline Name";
            Console.WriteLine("After setting custom name, IsNameAuto: " + trendline.IsNameAuto);
            
            // إعادة الضبط إلى الاسم التلقائي
            trendline.IsNameAuto = true;
            Console.WriteLine("After setting IsNameAuto=true, Name: " + trendline.Name);
        }
    }
}
```

### انظر أيضًا

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


