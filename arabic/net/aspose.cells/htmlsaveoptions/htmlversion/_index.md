---
title: "HtmlSaveOptions.HtmlVersion"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تحدد نسخة معيار HTML التي يجب استخدامها عند حفظ تنسيق HTML. القيمة الافتراضية هي HtmlVersion.Default"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/htmlversion/
---
## HtmlSaveOptions.HtmlVersion property

يحدد إصدار معيار HTML الذي يجب استخدامه عند حفظ الصيغة HTML. القيمة الافتراضية هي HtmlVersion.Default.

```csharp
public HtmlVersion HtmlVersion { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyHtmlVersionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion property");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["C4"].PutValue("Sample Text");
            
            // إنشاء كائن HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // عرض قيمة HtmlVersion الحالية
            Console.WriteLine("Current HtmlVersion: " + options.HtmlVersion);
            
            // تعيين HtmlVersion إلى HTML5
            options.HtmlVersion = HtmlVersion.Html5;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // حفظ باستخدام نسخة HTML5
            workbook.Save("HtmlVersion_Html5.html", options);
            
            // التغيير إلى XHTML
            options.HtmlVersion = HtmlVersion.XHtml;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // حفظ باستخدام نسخة XHTML
            workbook.Save("HtmlVersion_XHtml.html", options);
            
            // إعادة الضبط إلى الإعداد الافتراضي
            options.HtmlVersion = HtmlVersion.Default;
            Console.WriteLine("HtmlVersion reset to: " + options.HtmlVersion);
            
            // حفظ باستخدام النسخة الافتراضية
            workbook.Save("HtmlVersion_Default.html", options);
        }
    }
}
```

### انظر أيضًا

* enum [HtmlVersion](../../htmlversion/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


