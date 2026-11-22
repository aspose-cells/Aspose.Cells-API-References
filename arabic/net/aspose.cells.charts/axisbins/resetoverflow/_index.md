---
title: "AxisBins.ResetOverflow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AxisBins. إعادة تعيين الفائض"
type: docs
url: /ar/net/aspose.cells.charts/axisbins/resetoverflow/
---
## AxisBins.ResetOverflow method

إعادة تعيين الفائض

```csharp
[Obsolete("This is an internal method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ResetOverflow()
```

### ملاحظات

ملاحظة: هذه الطريقة الآن مهجورة. هذه طريقة داخلية لا تحتاج إلى استدعائها من الخارج لتجنب حدوث مشاكل. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2024. تتقدم Aspose بالاعتذار عن أي إزعاج قد تكون قد تعرضت له.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsMethodResetOverflowDemo
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

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على محور القيمة
            Axis valueAxis = chart.ValueAxis;

            // إنشاء حاويات المحور
            AxisBins bins = valueAxis.Bins;

            // تعيين قيمة الفائض
            bins.Overflow = 25;
            Console.WriteLine($"Overflow before reset: {bins.Overflow}");

            try
            {
                // استدعاء طريقة ResetOverflow
                bins.ResetOverflow();
                Console.WriteLine($"Overflow after reset: {bins.Overflow}");
                Console.WriteLine("ResetOverflow method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetOverflow method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("AxisBinsMethodResetOverflowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


