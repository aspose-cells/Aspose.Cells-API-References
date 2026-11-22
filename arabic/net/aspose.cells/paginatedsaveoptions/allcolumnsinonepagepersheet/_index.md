---
title: "PaginatedSaveOptions.AllColumnsInOnePagePerSheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. إذا كان AllColumnsInOnePagePerSheet صحيحًا، سيتم إخراج جميع محتويات الأعمدة لورقة واحدة في صفحة واحدة فقط في النتيجة. سيتم تجاهل عرض حجم الورق في إعدادات الصفحة وستظل الإعدادات الأخرى لإعداد الصفحة سارية."
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/
---
## PaginatedSaveOptions.AllColumnsInOnePagePerSheet property

إذا كان AllColumnsInOnePagePerSheet صحيحًا، فسيتم إخراج جميع محتويات الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيتم تجاهل عرض حجم الورق في pagesetup، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات نموذجية لتوضيح ملاءمة الأعمدة
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[0, i].PutValue("Column " + (i + 1));
                worksheet.Cells[1, i].PutValue("Sample data " + (i + 1));
            }

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;

            // حفظ المصنف باستخدام الخيارات
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with all columns in one page per sheet.");
        }
    }
}
```

### انظر أيضًا

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


