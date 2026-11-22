---
title: "Style.GetTwoColorGradientSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Style. الحصول على إعداد التدرج اللوني ثنائي اللون"
type: docs
url: /ar/net/aspose.cells/style/gettwocolorgradientsetting/
---
## Style.GetTwoColorGradientSetting method

احصل على إعداد التدرج اللوني ثنائي اللون.

```csharp
public TwoColorGradient GetTwoColorGradientSetting()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class StyleMethodGetTwoColorGradientSettingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط وتعيين تدرج لوني ثنائي
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);
            style.IsGradient = true;

            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Two Color Gradient Demo");
            cell.SetStyle(style);

            try
            {
                // استدعاء طريقة GetTwoColorGradientSetting
                TwoColorGradient gradientSetting = style.GetTwoColorGradientSetting();

                // عرض إعدادات التدرج
                Console.WriteLine("Color1: " + gradientSetting.Color1);
                Console.WriteLine("Color2: " + gradientSetting.Color2);
                Console.WriteLine("GradientStyleType: " + gradientSetting.GradientStyleType);
                Console.WriteLine("Variant: " + gradientSetting.Variant);

                // تعديل إعدادات التدرج
                gradientSetting.Color1 = Color.Green;
                gradientSetting.GradientStyleType = GradientStyleType.Vertical;
                style.SetTwoColorGradient(gradientSetting.Color1, gradientSetting.Color2, 
                                        gradientSetting.GradientStyleType, gradientSetting.Variant);

                Console.WriteLine("Gradient settings modified successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTwoColorGradientSetting method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("MethodGetTwoColorGradientSettingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TwoColorGradient](../../twocolorgradient/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


