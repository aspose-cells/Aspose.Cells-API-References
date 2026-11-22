---
title: "Axis.CustomUnit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تحدد قيمة مخصصة لوحدة العرض"
type: docs
url: /ar/net/aspose.cells.charts/axis/customunit/
---
## Axis.CustomUnit property

يحدد قيمة مخصصة لوحدة العرض.

```csharp
[Obsolete("Use Axis.CustomDisplayUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustomUnit { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهملة. بدلاً من ذلك، يرجى استخدام الخاصية Axis.CustomDisplayUnit. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustomUnitDemo
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
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // الوصول إلى محور القيم
                Axis valueAxis = chart.ValueAxis;

                // تعيين وحدة العرض إلى مخصصة
                valueAxis.DisplayUnit = DisplayUnitType.Custom;

                // تعيين قيمة وحدة العرض المخصصة
                valueAxis.CustomDisplayUnit = 1000000;

                // عرض قيمة الخاصية CustomUnit (خاصية مهملة)
                Console.WriteLine("CustomUnit value: " + valueAxis.CustomUnit);

                // احفظ المصنف
                workbook.Save("AxisPropertyCustomUnitDemo.xlsx");
                Console.WriteLine("CustomUnit has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


