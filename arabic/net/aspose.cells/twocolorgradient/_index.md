---
title: "فئة TwoColorGradient"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.TwoColorGradient فئة. يمثل تدرج لونين"
type: docs
url: /ar/net/aspose.cells/twocolorgradient/
---
## TwoColorGradient class

يمثل تدرج لونين.

```csharp
public class TwoColorGradient
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [TwoColorGradient](twocolorgradient/)(Color, Color, GradientStyleType, int) |  |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Color1](../../aspose.cells/twocolorgradient/color1/) { get; set; } | الحصول وتعيين لون التدرج الأول. |
| [Color2](../../aspose.cells/twocolorgradient/color2/) { get; set; } | الحصول وتعيين لون التدرج الثاني. |
| [GradientStyleType](../../aspose.cells/twocolorgradient/gradientstyletype/) { get; set; } | الحصول وتعيين نمط تظليل التدرج. |
| [Variant](../../aspose.cells/twocolorgradient/variant/) { get; set; } | الحصول وتعيين متغير التدرج. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class CellsClassTwoColorGradientDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تهيئة TwoColorGradient باستخدام معلمات المُنشئ
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightSkyBlue, 
                Color.DarkBlue, 
                GradientStyleType.DiagonalUp, 
                2);

            // تعديل خصائص التدرج بعد التهيئة
            gradient.GradientStyleType = GradientStyleType.DiagonalDown;

            // إنشاء نمط الخلية وتطبيق التدرج
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);

            // تطبيق النمط على الخلية وإضافة المحتوى
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Aspose.Cells TwoColorGradient Demo");
            cell.SetStyle(style);

            // ضبط أبعاد الخلية لتحسين الرؤية
            worksheet.Cells.SetRowHeight(1, 45);
            worksheet.Cells.SetColumnWidth(1, 55);

            // حفظ النتيجة مع تنسيق التدرج
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


