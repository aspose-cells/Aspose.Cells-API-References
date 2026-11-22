---
title: "الفئة GradientFill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.GradientFill. تمثل تعبئة التدرج اللوني"
type: docs
url: /ar/net/aspose.cells.drawing/gradientfill/
---
## GradientFill class

يمثل تعبئة التدرج.

```csharp
public class GradientFill : Fill
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Angle](../../aspose.cells.drawing/gradientfill/angle/) { get; set; } | زاوية التعبئة الخطية. |
| [DirectionType](../../aspose.cells.drawing/gradientfill/directiontype/) { get; } | يحصل على نوع اتجاه التدرج. |
| [FillType](../../aspose.cells.drawing/gradientfill/filltype/) { get; } | يحصل على نوع تعبئة التدرج. |
| [GradientStops](../../aspose.cells.drawing/gradientfill/gradientstops/) { get; } | يمثل مجموعة نقاط توقف التدرج. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(موروث من [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | الحصول على رمز التجزئة. (موروث من [`Fill`](../fill/).) |
| [SetGradient](../../aspose.cells.drawing/gradientfill/setgradient/)(GradientFillType, double, GradientDirectionType) | تعيين نوع تعبئة التدرج والاتجاه. |
| [SetOneColorGradient](../../aspose.cells.drawing/gradientfill/setonecolorgradient/)(Color, double, GradientStyleType, int) | يضبط الملء المحدد إلى تدرج بلون واحد. ينطبق فقط على Excel 2007. |
| [SetPresetThemeGradient](../../aspose.cells.drawing/gradientfill/setpresetthemegradient/)(PresetThemeGradientType, ThemeColorType) | يحدد تعبئة التدرج اللوني للموضوع المسبق. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | يضبط الملء المحدد إلى تدرج بلونين. ينطبق فقط على Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | يضبط الملء المحدد إلى تدرج بلونين. ينطبق فقط على Excel 2007. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassGradientFillDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل إلى ورقة العمل مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 150, 100);

            // تعيين نوع التعبئة إلى تدرج للوصول إلى خصائص تعبئة التدرج
            shape.Fill.FillType = FillType.Gradient;

            // الحصول على نسخة تعبئة التدرج الحالية من الشكل
            GradientFill gradientFill = shape.Fill.GradientFill;

            // تكوين التدرج بلونين باستخدام النسخة الحالية
            gradientFill.SetTwoColorGradient(
                Color.LightSkyBlue,  // First color
                Color.DarkBlue,      // Second color
                GradientStyleType.Horizontal, // Gradient style
                1                    // Variant
            );

            // احفظ المصنف
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


