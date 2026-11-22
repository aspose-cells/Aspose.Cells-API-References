---
title: "Chart.GetActualSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Chart. تحصل على الحجم الفعلي للمخطط بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.charts/chart/getactualsize/
---
## Chart.GetActualSize method

يحصل على الحجم الفعلي للمخطط بوحدة البكسل.

```csharp
public int[] GetActualSize()
```

### قيمة الإرجاع

الحجم الفعلي في مصفوفة (العرض والارتفاع). [0] هو العرض؛ [1] هو الارتفاع.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodGetActualSizeDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);
            
            try
            {
                // استدعِ طريقة GetActualSize
                int[] actualSize = chart.GetActualSize();
                
                // اعرض النتيجة
                Console.WriteLine($"Actual chart size - Width: {actualSize[0]}px, Height: {actualSize[1]}px");
                
                // أظهر التأثير عن طريق تغيير حجم كائن المخطط
                chart.ChartObject.Width = actualSize[0];
                chart.ChartObject.Height = actualSize[1];
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetActualSize method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("ChartMethodGetActualSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


