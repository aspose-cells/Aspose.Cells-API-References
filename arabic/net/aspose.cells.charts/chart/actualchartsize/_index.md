---
title: "Chart.ActualChartSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تحصل على الحجم الفعلي للمخطط بوحدات البكسل"
type: docs
url: /ar/net/aspose.cells.charts/chart/actualchartsize/
---
## Chart.ActualChartSize property

يحصل على الحجم الفعلي للمخطط بوحدات البكسل.

```csharp
[Obsolete("Use Chart.GetActualSize() method instead.")]
public Size ActualChartSize { get; }
```

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة Chart.GetActualSize(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2022. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyActualChartSizeDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // احسب المخطط لضمان تعبئة الخصائص
            chart.Calculate();

            // عرض استخدام ActualChartSize
            Console.WriteLine($"Actual Chart Size - Width: {chart.ActualChartSize.Width}, Height: {chart.ActualChartSize.Height}");

            // أضف شكلاً يكون حجمه مستندًا إلى ActualChartSize
            Shape shape = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle,
                PlacementType.Move,
                0.5,  // x position (relative)
                0.5,  // y position (relative)
                0.5 + (0.1 * chart.ActualChartSize.Height / chart.ActualChartSize.Width),  // width adjusted by aspect ratio
                0.6   // height
            );
            shape.Fill.SolidFill.Color = Color.Blue;

            // احفظ المصنف
            workbook.Save("ChartWithActualSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


