---
title: "ChartCalculateOptions.UpdateAllPoints"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartCalculateOptions. ما إذا كان يتم تحديث جميع نقاط البيانات عند إجراء حساب المخطط. القيمة الافتراضية False. عندما تريد الحصول على قيمة كل نقطة بيانات في المخطط، قم بتعيينها إلى true. إذا تم تعيين هذا المعامل إلى True قد يتم إنشاء نقاط بيانات جديدة عند حساب المخطط. هذا قد يجعل ملف Excel أكبر"
type: docs
url: /ar/net/aspose.cells.charts/chartcalculateoptions/updateallpoints/
---
## ChartCalculateOptions.UpdateAllPoints property

ما إذا كان يتم تحديث جميع نقاط البيانات عند إجراء حساب المخطط. الافتراضي: False. عندما تريد الحصول على قيمة كل نقطة بيانات في المخطط بشكل محدد، اضبطه على true. إذا تم تعيين هذه المعلمة إلى True، قد يتم إنشاء نقاط بيانات جديدة عند حساب المخطط. هذا قد يجعل ملف Excel أكبر.

```csharp
public bool UpdateAllPoints { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsPropertyUpdateAllPointsDemo
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
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(400);
            worksheet.Cells["C3"].PutValue(500);
            worksheet.Cells["C4"].PutValue(600);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // تمكين تسميات البيانات
            foreach (Aspose.Cells.Charts.Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
            }

            // احسب المخطط باستخدام خيار UpdateAllPoints
            chart.Calculate(new Aspose.Cells.Charts.ChartCalculateOptions() { UpdateAllPoints = true });

            // إخراج بعض قيم تسميات البيانات لتوضيح النتيجة
            Console.WriteLine("Series1 Point1 Label: " + chart.NSeries[0].Points[0].DataLabels.Text);
            Console.WriteLine("Series2 Point2 Label: " + chart.NSeries[1].Points[1].DataLabels.Text);
        }
    }
}
```

### انظر أيضًا

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


