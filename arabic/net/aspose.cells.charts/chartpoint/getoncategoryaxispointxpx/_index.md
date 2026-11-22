---
title: "ChartPoint.GetOnCategoryAxisPointXPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartPoint. تحصل على إحداثي x للنقطة على محور الفئة بعد استدعاء طريقة Chart.Calculate. تنطبق فقط على مخطط المنطقة"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/getoncategoryaxispointxpx/
---
## ChartPoint.GetOnCategoryAxisPointXPx method

يحصل على إحداثي x للنقطة على محور الفئة بعد استدعاء طريقة Chart.Calculate(). ينطبق فقط على مخطط المنطقة.

```csharp
public float GetOnCategoryAxisPointXPx(int index)
```

### ملاحظات

مخطط المنطقة ثنائي الأبعاد: الفهرس هو 0. مخطط المنطقة ثلاثي الأبعاد: الفهرس هو 0 أو 1.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointXPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // حساب المخطط
            chart.Calculate();

            try
            {
                // احصل على أول نقطة في المخطط
                ChartPoint point = chart.NSeries[0].Points[0];

                // استدعِ GetOnCategoryAxisPointXPx مع الفهرس 0
                float xPosition = point.GetOnCategoryAxisPointXPx(0);

                // اعرض النتيجة
                Console.WriteLine($"X position of first category axis point: {xPosition} pixels");

                // احفظ المصنف
                workbook.Save("ChartPointGetOnCategoryAxisPointXPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointXPx method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


