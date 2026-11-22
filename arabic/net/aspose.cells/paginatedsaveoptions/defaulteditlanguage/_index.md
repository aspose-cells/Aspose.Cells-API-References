---
title: "PaginatedSaveOptions.DefaultEditLanguage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تحصل أو تعيين لغة التحرير الافتراضية"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/defaulteditlanguage/
---
## PaginatedSaveOptions.DefaultEditLanguage property

يحصل أو يضبط لغة التحرير الافتراضية.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### ملاحظات

قد يعرض/يرسم تخطيطات مختلفة لفقرة النص عندما يتم تعيين لغات تحرير مختلفة. الافتراضي هو Auto.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض النصوص CJK لتوضيح خاصية DefaultEditLanguage
            worksheet.Cells["A1"].PutValue("日本語のテキスト");
            worksheet.Cells["A2"].PutValue("中文文本");
            worksheet.Cells["A3"].PutValue("한글 텍스트");

            // أنشئ خيارات حفظ PDF واضبط CJK كلغة تحرير افتراضية
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
            
            // احفظ المصنف باستخدام الخيارات المحددة
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("Workbook saved with CJK as default edit language.");
        }
    }
}
```

### انظر أيضًا

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


