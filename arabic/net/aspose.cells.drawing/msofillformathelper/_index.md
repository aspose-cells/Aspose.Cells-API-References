---
title: "فئة MsoFillFormatHelper"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.MsoFillFormatHelper. يمثل تنسيق التعبئة لشكل"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformathelper/
---
## MsoFillFormatHelper class

يمثل تنسيق التعبئة لشكل.

```csharp
public class MsoFillFormatHelper
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformathelper/backcolor/) { get; set; } | يحصل ويضبط لون الخلفية للملف. |
| [ForeColor](../../aspose.cells.drawing/msofillformathelper/forecolor/) { get; set; } | يحصل ويضبط لون المقدمة للتعبئة. |
| [ForeColorTransparency](../../aspose.cells.drawing/msofillformathelper/forecolortransparency/) { get; set; } | إرجاع أو تعيين درجة اللون الأمامي للملء المحدد كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [ImageData](../../aspose.cells.drawing/msofillformathelper/imagedata/) { get; set; } | الحصول على وتعيين بيانات ملء النسيج والصورة. |
| [IsVisible](../../aspose.cells.drawing/msofillformathelper/isvisible/) { get; set; } | يشير إلى ما إذا كان هناك ملء. |
| [Texture](../../aspose.cells.drawing/msofillformathelper/texture/) { get; } | الحصول على نوع ملء النسيج. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformathelper/setonecolorgradient/)(Color, double, GradientStyleType, int) | تعيين الملء المحدد إلى تدرج لون واحد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.Reflection;

    public class DrawingClassMsoFillFormatHelperDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "MsoFillFormatHelper Demo";

            try
            {
                // إنشاء نسخة من MsoFillFormatHelper باستخدام الانعكاس
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // تعيين الخصائص الأساسية
                fillHelper.ForeColor = Color.FromArgb(255, 100, 150, 200);
                fillHelper.ForeColorTransparency = 0.3;
                fillHelper.BackColor = Color.LightGray;
                fillHelper.IsVisible = true;

                // عرض قيم الخصائص
                Console.WriteLine($"ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency: {fillHelper.ForeColorTransparency}");
                Console.WriteLine($"BackColor: {fillHelper.BackColor}");
                Console.WriteLine($"IsVisible: {fillHelper.IsVisible}");
                Console.WriteLine($"Texture (read-only): {fillHelper.Texture}");

                // احفظ المصنف
                workbook.Save("MsoFillFormatHelperDemo.xlsx");
                Console.WriteLine("MsoFillFormatHelper demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in MsoFillFormatHelper demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


