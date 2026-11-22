---
title: "HtmlSaveOptions.DisableCss"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كانت الأنماط المضمنة فقط تُطبق دون الاعتماد على CSS. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/disablecss/
---
## HtmlSaveOptions.DisableCss property

يشير إلى ما إذا كانت الأنماط المضمنة فقط تُطبق، دون الاعتماد على CSS. القيمة الافتراضية هي false.

```csharp
public bool DisableCss { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyDisableCssDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة وتنسيق
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["B1"].PutValue("Formatted Cell");
            worksheet.Cells["B1"].GetStyle().Font.IsItalic = true;
            worksheet.Cells["B1"].GetStyle().Font.Underline = FontUnderlineType.Single;

            // إنشاء كائن HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();

            // عرض قيمة DisableCss الحالية
            Console.WriteLine("Current DisableCss value: " + options.DisableCss);

            // تعيين DisableCss إلى true (باستخدام الأنماط المضمنة بدلاً من CSS)
            options.DisableCss = true;
            workbook.Save("HtmlWithInlineStyles.html", options);

            // تعيين DisableCss إلى false (باستخدام أنماط CSS)
            options.DisableCss = false;
            workbook.Save("HtmlWithCssStyles.html", options);

            // قارن ملفات الإخراج لرؤية الفرق في نهج التنسيق
            Console.WriteLine("Files saved with different DisableCss settings.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


