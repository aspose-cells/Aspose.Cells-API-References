---
title: "ChartFrame.SetPositionAuto"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartFrame. اضبط موضع الإطار إلى تلقائي"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/setpositionauto/
---
## ChartFrame.SetPositionAuto method

تعيين موقع الإطار إلى تلقائي

```csharp
public virtual void SetPositionAuto()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFrameMethodSetPositionAutoDemo
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

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على إطار عنوان المخطط
            ChartFrame title = chart.Title;
            
            // اضبط الموضع اليدوي أولاً لتوضيح SetPositionAuto
            title.XRatioToChart = 0.2;
            title.YRatioToChart = 0.1;
            title.WidthRatioToChart = 0.6;
            title.HeightRatioToChart = 0.1;

            try
            {
                // استدعِ طريقة SetPositionAuto
                title.SetPositionAuto();
                
                Console.WriteLine("Chart title position set to automatic successfully");
                
                // عرض قيم الموضع التلقائي الجديدة
                Console.WriteLine($"New X position ratio: {title.XRatioToChart}");
                Console.WriteLine($"New Y position ratio: {title.YRatioToChart}");
                Console.WriteLine($"New Width ratio: {title.WidthRatioToChart}");
                Console.WriteLine($"New Height ratio: {title.HeightRatioToChart}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("ChartFrameSetPositionAutoDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


