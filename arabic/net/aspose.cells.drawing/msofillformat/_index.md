---
title: "الفئة MsoFillFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.MsoFillFormat. تمثل تنسيق التعبئة لشكل"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformat/
---
## MsoFillFormat class

يمثل تنسيق التعبئة لشكل.

```csharp
public class MsoFillFormat
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformat/backcolor/) { get; set; } | يحصل ويضبط لون الخلفية للملف. |
| [ForeColor](../../aspose.cells.drawing/msofillformat/forecolor/) { get; set; } | يحصل ويضبط لون المقدمة للتعبئة. |
| [ImageData](../../aspose.cells.drawing/msofillformat/imagedata/) { get; set; } | الحصول على وتعيين بيانات ملء النسيج والصورة. |
| [IsVisible](../../aspose.cells.drawing/msofillformat/isvisible/) { get; set; } | يشير إلى ما إذا كان هناك ملء. |
| [Texture](../../aspose.cells.drawing/msofillformat/texture/) { get; } | الحصول على نوع ملء النسيج. |
| [Transparency](../../aspose.cells.drawing/msofillformat/transparency/) { get; set; } | إرجاع أو تعيين درجة الشفافية للملء المحدد كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | تعيين الملء المحدد إلى تدرج لون واحد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatDemo
    {
        public static void MsoFillFormatExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً قوسيًا إلى ورقة العمل
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // الوصول إلى تنسيق التعبئة للشكل
            MsoFillFormat fillFormat = arcShape.FillFormat;

            // تعيين لون مقدمة التعبئة
            fillFormat.ForeColor = Color.Blue;

            // تعيين لون خلفية التعبئة
            fillFormat.BackColor = Color.LightBlue;

            // تعيين الشفافية
            fillFormat.Transparency = 0.5;

            // تحقق مما إذا كانت التعبئة مرئية
            bool isVisible = fillFormat.IsVisible;
            Console.WriteLine("Is Fill Visible: " + isVisible);

            // تعيين تعبئة تدرج لوني بلون واحد
            fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);

            // احفظ المصنف
            workbook.Save("MsoFillFormatExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


