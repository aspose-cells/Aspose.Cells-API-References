---
title: "PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد شيء للطباعة"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/
---
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property

يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد ما للطباعة.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل وأخفها (محاكاة عدم وجود شيء للطباعة)
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.IsVisible = false;

            // حدد خيارات حفظ PDF مع OutputBlankPageWhenNothingToPrint = false
            PdfSaveOptions options = new PdfSaveOptions
            {
                OutputBlankPageWhenNothingToPrint = false
            };

            // احفظ كملف PDF - لا يجب إنشاء صفحة فارغة
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputNoBlankPage.pdf");
            workbook.Save(outputPath, options);

            // غيّر الخيار إلى true
            options.OutputBlankPageWhenNothingToPrint = true;

            // احفظ مرة أخرى - يجب إنشاء صفحة فارغة
            outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputWithBlankPage.pdf");
            workbook.Save(outputPath, options);
        }
    }
}
```

### انظر أيضًا

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


