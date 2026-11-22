---
title: "TwoColorGradient.Variant"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TwoColorGradient. تحصل وتضبط متغير التدرج"
type: docs
url: /ar/net/aspose.cells/twocolorgradient/variant/
---
## TwoColorGradient.Variant property

الحصول وتعيين متغير التدرج.

```csharp
public int Variant { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء تدرج لوني ثنائي اللون مع المتغير الأولي
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.DarkBlue,
                GradientStyleType.Horizontal,
                1
            );

            // إنشاء وتطبيق النمط على الخلية A1
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Variant 1");

            // عرض قيمة المتغير الحالية
            System.Console.WriteLine("Current Variant value: " + gradient.Variant);

            // تعديل قيمة المتغير
            gradient.Variant = 2;

            // إنشاء وتطبيق النمط المعدل على الخلية B1
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Variant 2");

            // زيادة ارتفاع الخلايا لتصوير التدرجات
            worksheet.Cells.Rows[0].Height = 150;

            workbook.Save("TwoColorGradientVariantDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


