---
title: "PaginatedSaveOptions.TextCrossType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تحصل أو تعين نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/textcrosstype/
---
## PaginatedSaveOptions.TextCrossType property

يحصل أو يضبط نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن نصًا طويلًا سيتجاوز حدود الخلية
            worksheet.Cells["A1"].PutValue("This is a long text that will cross cell boundaries");
            worksheet.Cells["B1"].PutValue("Another cell content");
            
            // عيّن عرض العمود لجعل النص يتجاوز الخلايا
            worksheet.Cells.SetColumnWidth(0, 5);
            
            // أنشئ خيارات حفظ PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // أظهر TextCrossType بتعيينه إلى CrossKeep
            options.TextCrossType = TextCrossType.CrossKeep;
            
            // احفظ المصنف كملف PDF
            workbook.Save("TextCrossTypeDemo.pdf", options);
            
            Console.WriteLine("PDF saved with TextCrossType.CrossKeep setting");
        }
    }
}
```

### انظر أيضًا

* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


