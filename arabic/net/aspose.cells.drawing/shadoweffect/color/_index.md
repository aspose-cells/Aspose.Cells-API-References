---
title: "ShadowEffect.Color"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShadowEffect. تحصل وتعيّن لون الظل"
type: docs
url: /ar/net/aspose.cells.drawing/shadoweffect/color/
---
## ShadowEffect.Color property

الحصول وتعيين لون الظل.

```csharp
public CellsColor Color { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShadowEffectPropertyColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل لإظهار تأثير الظل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // الحصول على تأثير الظل من الشكل
                ShadowEffect shadowEffect = shape.ShadowEffect;

                // إنشاء كائن CellsColor جديد
                CellsColor shadowColor = workbook.CreateCellsColor();

                // تعيين اللون إلى الأحمر باستخدام قيم RGB
                shadowColor.Color = Color.Red;

                // تطبيق اللون على تأثير الظل
                shadowEffect.Color = shadowColor;

                // عرض قيمة اللون الحالية
                Console.WriteLine("Shadow Color (RGB): " + shadowEffect.Color.Color.ToString());
                Console.WriteLine("Shadow Color (ARGB): " + shadowEffect.Color.Argb);

                // احفظ المصنف لتوضيح التأثير
                workbook.Save("ShadowEffectColorDemo.xlsx");

                // تحميل المصنف مرة أخرى للتحقق من حفظ اللون
                Workbook loadedWorkbook = new Workbook("ShadowEffectColorDemo.xlsx");
                ShadowEffect loadedShadowEffect = loadedWorkbook.Worksheets[0].Shapes[0].ShadowEffect;

                // عرض قيمة اللون التي تم تحميلها
                Console.WriteLine("Loaded Shadow Color (RGB): " + loadedShadowEffect.Color.Color.ToString());
                Console.WriteLine("Loaded Shadow Color (ARGB): " + loadedShadowEffect.Color.Argb);
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


