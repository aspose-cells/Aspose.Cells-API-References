---
title: "MsoFillFormatHelper.SetOneColorGradient"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة MsoFillFormatHelper. تقوم بتعيين التعبئة المحددة إلى تدرج لون واحد"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformathelper/setonecolorgradient/
---
## MsoFillFormatHelper.SetOneColorGradient method

تعيين الملء المحدد إلى تدرج لون واحد.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اللون | اللون | لون تدرج واحد. |
| درجة | Double | درجة التدرج. يمكن أن تكون قيمة من 0.0 (غامق) إلى 1.0 (فاتح). |
| النمط | GradientStyleType | نمط تظليل التدرج. |
| variant | Int32 | متغير التدرج. يمكن أن يكون قيمة من 1 إلى 4، المقابل لأحد المتغيرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان style هو GradientStyle.FromCenter، فإن معامل Variant لا يمكن أن يكون إلا 1 أو 2. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ضع تسمية بسيطة في الورقة للتوضيح
            worksheet.Cells["A1"].Value = "Gradient Fill Demo";

            try
            {
                // إنشاء نسخة من MsoFillFormatHelper باستخدام الانعكاس (بدون مُنشئ عام)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // معلمات التدرج
                Color gradientColor = Color.FromArgb(255, 0, 120, 215); // a shade of blue
                double degree = 45.0;                                 // gradient angle in degrees
                GradientStyleType style = GradientStyleType.Horizontal; // horizontal gradient
                int variant = 0;                                      // variant (0 = default)

                // تطبيق تدرج اللون الواحد
                fillHelper.SetOneColorGradient(gradientColor, degree, style, variant);

                // اختياري: إظهار أن الخصائص يمكن قراءةها بعد الاستدعاء
                Console.WriteLine($"ForeColor after gradient: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency after gradient: {fillHelper.ForeColorTransparency}");

                // احفظ المصنف (لن يُلاحظ أي تغيير بصري لأن المساعد غير مُرفق بشكل).
                workbook.Save("SetOneColorGradientDemo.xlsx");

                Console.WriteLine("SetOneColorGradient method called successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


