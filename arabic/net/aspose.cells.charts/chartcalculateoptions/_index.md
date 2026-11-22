---
title: "الفئة ChartCalculateOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.ChartCalculateOptions. تمثل الخيارات لحساب مخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartcalculateoptions/
---
## ChartCalculateOptions class

يمثل الخيارات لحساب المخطط.

```csharp
public class ChartCalculateOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ChartCalculateOptions](chartcalculateoptions/)() | ينشئ الخيارات لحساب المخطط. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [UpdateAllPoints](../../aspose.cells.charts/chartcalculateoptions/updateallpoints/) { get; set; } | ما إذا كان يتم تحديث جميع نقاط البيانات عند إجراء حساب المخطط. الافتراضي: False. عندما تريد الحصول على قيمة كل نقطة بيانات في المخطط بشكل محدد، اضبطه على true. إذا تم تعيين هذه المعلمة إلى True، قد يتم إنشاء نقاط بيانات جديدة عند حساب المخطط. هذا قد يجعل ملف Excel أكبر. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCalculateOptionsDemo
    {
        public static void ChartCalculateOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تحديد نطاق البيانات للمخطط
            chart.SetChartDataRange("A1:B4", true);

            // إنشاء مثال من ChartCalculateOptions
            ChartCalculateOptions options = new ChartCalculateOptions
            {
                UpdateAllPoints = true // Set the property to update all data points
            };

            // احسب المخطط باستخدام الخيارات المحددة
            chart.Calculate(options);

            // احفظ المصنف
            workbook.Save("ChartCalculateOptionsExample.xlsx");
            workbook.Save("ChartCalculateOptionsExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


