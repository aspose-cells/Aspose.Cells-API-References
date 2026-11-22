---
title: "Style.SetTwoColorGradient"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Style. تعيين التعبئة المحددة إلى تدرج لوني ثنائي"
type: docs
url: /ar/net/aspose.cells/style/settwocolorgradient/
---
## Style.SetTwoColorGradient method

يضبط التعبئة المحددة لتصبح تدرجًا لونيًا ثنائي اللون.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| color1 | اللون | لون تدرج واحد. |
| color2 | اللون | لونين تدرج. |
| gradientStyleType | GradientStyleType | نمط تظليل التدرج. |
| variant | Int32 | متغير التدرج. يمكن أن يكون قيمة من 1 إلى 4، المقابل لأحد المتغيرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان style هو GradientStyle.FromCenter، فإن معامل Variant لا يمكن أن يكون إلا 1 أو 2. |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن نمط
            Style style = workbook.CreateStyle();

            // تعيين تدرج لوني ثنائي للنمط
            style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);

            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Gradient Style Demo");

            // تحقق من إعدادات التدرج
            Color color1, color2;
            GradientStyleType gradientStyle;
            int variant;
            style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);

            Console.WriteLine("Color1: " + color1);
            Console.WriteLine("Color2: " + color2);
            Console.WriteLine("Gradient Style: " + gradientStyle);
            Console.WriteLine("Variant: " + variant);

            // احفظ المصنف
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


