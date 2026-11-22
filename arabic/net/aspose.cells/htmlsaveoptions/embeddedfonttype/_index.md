---
title: "HtmlSaveOptions.EmbeddedFontType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "HtmlSaveOptions property. تحصل أو تعيين نوع تضمين ملف الخط في ملف html. القيمة الافتراضية هي None والتي تشير إلى عدم تضمين أي خط في html"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/embeddedfonttype/
---
## HtmlSaveOptions.EmbeddedFontType property

يحصل على أو يضبط نوع تضمين ملف الخط في ملف html. القيمة الافتراضية هي None والتي تشير إلى عدم تضمين أي خط في html.

```csharp
public HtmlEmbeddedFontType EmbeddedFontType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Sample Text with Font");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);

            try
            {
                // إنشاء خيارات حفظ HTML
                HtmlSaveOptions options = new HtmlSaveOptions();

                // عرض قيمة EmbeddedFontType الافتراضية
                Console.WriteLine("Default EmbeddedFontType: " + options.EmbeddedFontType);

                // تعيين EmbeddedFontType إلى Woff
                options.EmbeddedFontType = HtmlEmbeddedFontType.Woff;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // حفظ المصنف مع تضمين خط WOFF
                workbook.Save("EmbeddedFontType_Woff.html", options);

                // إعادة الضبط إلى None
                options.EmbeddedFontType = HtmlEmbeddedFontType.None;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // حفظ المصنف بدون تضمين الخط
                workbook.Save("EmbeddedFontType_None.html", options);

                Console.WriteLine("EmbeddedFontType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [HtmlEmbeddedFontType](../../../aspose.cells.rendering/htmlembeddedfonttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


