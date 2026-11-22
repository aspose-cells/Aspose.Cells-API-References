---
title: "Line.GradientFill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Line. تمثل تعبئة التدرج"
type: docs
url: /ar/net/aspose.cells.drawing/line/gradientfill/
---
## Line.GradientFill property

يمثل تعبئة متدرجة.

```csharp
public GradientFill GradientFill { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;

    public class LinePropertyGradientFillDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض بيانات العينة للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // احصل على النقطة الأولى للسلسلة الأولى
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            try
            {
                // الوصول إلى كائن Line (الحد) للنقطة
                Line line = point.Border;

                // قراءة خاصية GradientFill (للقراءة فقط)
                GradientFill gradient = line.GradientFill;

                // عرض تفاصيل تعبئة التدرج الحالية
                Console.WriteLine("Current GradientFill:");
                Console.WriteLine($"  FillType       = {gradient.FillType}");
                Console.WriteLine($"  DirectionType = {gradient.DirectionType}");
                Console.WriteLine($"  Angle          = {gradient.Angle}");

                // تعديل التدرج باستخدام الطرق المقدمة
                // استخدم تحويلًا إلى قيمة تعداد افتراضية لتجنب الإشارة إلى عضو غير موجود
                gradient.SetGradient(GradientFillType.Linear, 45.0, (GradientDirectionType)0);
                Console.WriteLine("GradientFill after SetGradient:");
                Console.WriteLine($"  Angle = {gradient.Angle}");

                // احفظ المصنف
                workbook.Save("LinePropertyGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [GradientFill](../../gradientfill/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


