---
title: "PdfSaveOptions.EmbedStandardWindowsFonts"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. True لتضمين خطوط TrueType. يؤثر فقط على أحرف ASCII 32127. الخطوط لأكواد الأحرف التي تزيد عن 127 يتم تضمينها دائمًا. الخطوط دائمًا ما تُضمّن للمعايير PDF/A1a و PDF/A1b. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/
---
## PdfSaveOptions.EmbedStandardWindowsFonts property

True لتضمين خطوط True type fonts. يؤثر فقط على أحرف ASCII 32-127. الخطوط للأكواد التي تزيد عن 127 يتم تضمينها دائمًا. الخطوط يتم تضمينها دائمًا لمعيار PDF/A-1a و PDF/A-1b. القيمة الافتراضية هي true.

```csharp
public bool EmbedStandardWindowsFonts { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedStandardWindowsFontsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF with embedded fonts");

            // عيّن خيارات حفظ PDF مع خاصية EmbedStandardWindowsFonts
            PdfSaveOptions options = new PdfSaveOptions();
            options.EmbedStandardWindowsFonts = true;

            // حفظ إلى تدفق الذاكرة
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved with embedded fonts: " + (ms.Length > 0));
            }

            // أظهر تعطيل تضمين الخطوط
            options.EmbedStandardWindowsFonts = false;
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved without embedded fonts: " + (ms.Length > 0));
            }
        }
    }
}
```

### انظر أيضًا

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


