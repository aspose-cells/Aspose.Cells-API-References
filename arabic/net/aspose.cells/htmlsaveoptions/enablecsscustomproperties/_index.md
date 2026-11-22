---
title: "HtmlSaveOptions.EnableCssCustomProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "HtmlSaveOptions property. تحسين مخرجات html باستخدام خصائص CSS المخصصة. على سبيل المثال، في السيناريو الذي توجد فيه تكرارات متعددة لصورة base64 واحدة مع خاصية مخصصة، تحتاج بيانات الصورة إلى الحفظ مرة واحدة فقط، وبالتالي يمكن تحسين أداء html الناتج. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/enablecsscustomproperties/
---
## HtmlSaveOptions.EnableCssCustomProperties property

حسّن مخرجات html باستخدام خصائص CSS المخصصة. على سبيل المثال، في السيناريو الذي توجد فيه تكرارات متعددة لصورة base64 واحدة، مع الخاصية المخصصة يحتاج بيانات الصورة أن تُحفظ مرة واحدة فقط وبالتالي يمكن تحسين أداء html الناتج. القيمة الافتراضية هي false.

```csharp
public bool EnableCssCustomProperties { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyEnableCssCustomPropertiesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية مع التنسيق
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;

            // إضافة صورة سيتم تكرارها في خلايا متعددة
            int imgIndex = worksheet.Pictures.Add(1, 1, "logo.png");
            Picture pic = worksheet.Pictures[imgIndex];
            pic.Move(1, 1); // Using Move instead of LeftOffset/TopOffset
            pic.Width = 100;
            pic.Height = 100;

            // نسخ الصورة إلى موقع آخر
            worksheet.Cells["D5"].PutValue("Same image reference:");
            int imgIndex2 = worksheet.Pictures.Add(5, 3, "logo.png");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            pic2.Move(5, 3); // Using Move instead of LeftOffset/TopOffset
            pic2.Width = 100;
            pic2.Height = 100;

            // إنشاء كائن HtmlSaveOptions
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

            // عرض القيمة الحالية
            Console.WriteLine("Current EnableCssCustomProperties value: " + htmlOptions.EnableCssCustomProperties);

            // اضبطه على true لتحسين مخرجات CSS
            htmlOptions.EnableCssCustomProperties = true;

            // احفظ مع تحسين CSS
            workbook.Save("HtmlWithCssCustomProperties.html", htmlOptions);

            // اضبطه على false للمقارنة
            htmlOptions.EnableCssCustomProperties = false;
            workbook.Save("HtmlWithoutCssCustomProperties.html", htmlOptions);

            Console.WriteLine("Files saved with and without CSS custom properties optimization.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


