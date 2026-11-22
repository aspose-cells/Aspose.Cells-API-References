---
title: "AxisBins.ResetUnderflow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AxisBins. إعادة تعيين الفائض السالب"
type: docs
url: /ar/net/aspose.cells.charts/axisbins/resetunderflow/
---
## AxisBins.ResetUnderflow method

إعادة تعيين الفائض السالب

```csharp
[Obsolete("This is an internal method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ResetUnderflow()
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

    public class AxisBinsMethodResetUnderflowDemo
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
            valueAxis.Bins.IsAutomatic = false;
            valueAxis.Bins.Count = 5;
            valueAxis.Bins.Underflow = 5;
            
            try
            {
                // استدعاء طريقة ResetUnderflow
                valueAxis.Bins.ResetUnderflow();
                
                Console.WriteLine("Underflow value after reset: " + valueAxis.Bins.Underflow);
                
                // احفظ المصنف
                workbook.Save("AxisBinsMethodResetUnderflowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetUnderflow method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


