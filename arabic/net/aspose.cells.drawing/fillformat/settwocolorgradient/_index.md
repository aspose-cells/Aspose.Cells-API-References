---
title: "FillFormat.SetTwoColorGradient"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FillFormat. تضبط الملء المحدد إلى تدرج لوني ثنائي. تنطبق فقط على Excel 2007"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/settwocolorgradient/
---
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}

يضبط الملء المحدد إلى تدرج بلونين. ينطبق فقط على Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| color1 | اللون | لون تدرج واحد. |
| color2 | اللون | لونين تدرج. |
| النمط | GradientStyleType | نمط تظليل التدرج. |
| variant | Int32 | متغير التدرج. يمكن أن يكون قيمة من 1 إلى 4، المقابل لأحد المتغيرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان style هو GradientStyle.FromCenter، فإن معامل Variant لا يمكن أن يكون إلا 1 أو 2. |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل بسيط لتوضيح ملء التدرج
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 100, 100);

            // احصل على تنسيق الملء للشكل
            FillFormat fillFormat = shape.Fill;

            // تعيين تدرج لوني ثنائي باستخدام المعلمات المحددة
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);

            // احفظ المصنف
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}

يضبط الملء المحدد إلى تدرج بلونين. ينطبق فقط على Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2, 
    double transparency2, GradientStyleType style, int variant)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| color1 | اللون | لون تدرج واحد. |
| transparency1 | Double | درجة شفافية اللون1 كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| color2 | اللون | لونين تدرج. |
| transparency2 | Double | درجة شفافية اللون2 كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
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

    public class FillFormatMethodSetTwoColorGradientWithColorDoubleColorDoubleGradientDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل مستطيل لتوضيح تنسيق الملء
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 150, 100);
            FillFormat fillFormat = rectangle.Fill;

            try
            {
                // تحضير المعلمات لـ SetTwoColorGradient
                Color color1 = Color.Red;
                double transparency1 = 0.3;
                Color color2 = Color.Blue;
                double transparency2 = 0.7;
                GradientStyleType gradientStyle = GradientStyleType.Horizontal;
                int variant = 1;

                // استدعاء SetTwoColorGradient بمعلمات محددة
                fillFormat.SetTwoColorGradient(
                    color1, 
                    transparency1, 
                    color2, 
                    transparency2, 
                    gradientStyle, 
                    variant
                );

                Console.WriteLine("SetTwoColorGradient executed successfully with parameters (Color, Double, Color, Double, GradientStyleType, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTwoColorGradient: {ex.Message}");
            }

            // احفظ المصنف لإظهار التأثير
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


