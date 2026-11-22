---
title: "FillFormat.GradientFill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. يحصل على كائن GradientFill"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/gradientfill/
---
## FillFormat.GradientFill property

يحصل على كائن `GradientFill`.

```csharp
public GradientFill GradientFill { get; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientFillDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // توفير بعض البيانات لمخطط
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // أضف مخطط عمودي
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // الوصول إلى تنسيق التعبئة لمنطقة السلسلة الأولى
                FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;

                // تطبيق تدرج لونين على السلسلة
                fillFormat.SetTwoColorGradient(Color.Red, Color.Blue,
                                               GradientStyleType.Horizontal, 2);

                // استرجاع كائن GradientFill (خاصية للقراءة فقط)
                GradientFill gradientFill = fillFormat.GradientFill;

                // عرض بعض المعلومات حول تعبئة التدرج
                Console.WriteLine("GradientFill details:");
                Console.WriteLine($"  FillType      : {gradientFill.FillType}");
                Console.WriteLine($"  DirectionType: {gradientFill.DirectionType}");
                Console.WriteLine($"  Angle         : {gradientFill.Angle}");

                // اختياريًا تعديل زاوية التدرج باستخدام مُحدد set
                gradientFill.Angle = 45.0f;
                Console.WriteLine($"  New Angle set to: {gradientFill.Angle}");

                // احفظ المصنف
                workbook.Save("FillFormatGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved as FillFormatGradientFillDemo.xlsx");
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
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


