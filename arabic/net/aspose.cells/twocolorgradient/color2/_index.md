---
title: "TwoColorGradient.Color2"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TwoColorGradient. يسترجع ويعيّن اللون الثاني للتدرج"
type: docs
url: /ar/net/aspose.cells/twocolorgradient/color2/
---
## TwoColorGradient.Color2 property

الحصول وتعيين لون التدرج الثاني.

```csharp
public Color Color2 { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor2Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن تدرج ثنائي اللون
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.Green,
                GradientStyleType.Horizontal,
                1);

            // إنشاء النمط الأول مع التدرج الأولي
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].PutValue("Initial Gradient");
            worksheet.Cells["A1"].SetStyle(style1);

            // عرض قيمة Color2 الحالية
            System.Console.WriteLine("Current Color2: " + gradient.Color2);

            // تعديل خاصية Color2
            gradient.Color2 = Color.Red;

            // إنشاء النمط الثاني مع التدرج المعدل
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A2"].PutValue("Modified Gradient");
            worksheet.Cells["A2"].SetStyle(style2);

            // ضبط الصفوف للظهور
            worksheet.Cells.SetRowHeight(0, 40);
            worksheet.Cells.SetRowHeight(1, 40);

            // احفظ المصنف
            workbook.Save("TwoColorGradientColor2Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


