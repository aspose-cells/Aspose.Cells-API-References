---
title: "MarkdownSaveOptions.ExportImagesAsBase64"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MarkdownSaveOptions. تحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى Markdown. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/markdownsaveoptions/exportimagesasbase64/
---
## MarkdownSaveOptions.ExportImagesAsBase64 property

يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى Markdown. القيمة الافتراضية هي true.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### ملاحظات

عند ضبط هذه الخاصية على true يتم تصدير بيانات الصورة مباشرةً على عناصر img ولا يتم إنشاء ملفات منفصلة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة وصورة
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("With Image");

            // إضافة صورة إلى ورقة العمل
            int imageIndex = worksheet.Pictures.Add(1, 1, "sample.png");

            try
            {
                // إنشاء مثيل MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // اعرض القيمة الافتراضية لـ ExportImagesAsBase64
                Console.WriteLine("Default ExportImagesAsBase64 value: " + saveOptions.ExportImagesAsBase64);

                // عيّن ExportImagesAsBase64 إلى false لتوضيح الخاصية
                saveOptions.ExportImagesAsBase64 = false;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // احفظ مع ExportImagesAsBase64 = false
                workbook.Save("MarkdownImagesAsFiles.md", saveOptions);

                // عيّن ExportImagesAsBase64 إلى true
                saveOptions.ExportImagesAsBase64 = true;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // احفظ مع ExportImagesAsBase64 = true
                workbook.Save("MarkdownImagesAsBase64.md", saveOptions);

                Console.WriteLine("Markdown files saved with different ExportImagesAsBase64 settings.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


