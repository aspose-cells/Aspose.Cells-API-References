---
title: "HtmlSaveOptions.ExportImagesAsBase64"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى HTML أو MHTML أو EPUB"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportimagesasbase64/
---
## HtmlSaveOptions.ExportImagesAsBase64 property

يحدد ما إذا كانت الصور تُحفظ بصيغة Base64 إلى HTML أو MHTML أو EPUB.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### ملاحظات

عند ضبط هذه الخاصية على true يتم تصدير بيانات الصورة مباشرةً على عناصر img ولا يتم إنشاء ملفات منفصلة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة صورة إلى ورقة العمل
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // ضبط ExportImagesAsBase64 على true لتضمين الصور كسلاسل base64
            saveOptions.ExportImagesAsBase64 = true;
            
            // حفظ المصنف كملف HTML مع صور مدمجة
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML with embedded images saved successfully.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


