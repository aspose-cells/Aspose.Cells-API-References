---
title: "PdfBookmarkEntry.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfBookmarkEntry. عنوان العلامة المرجعية"
type: docs
url: /ar/net/aspose.cells.rendering/pdfbookmarkentry/text/
---
## PdfBookmarkEntry.Text property

عنوان إشارة مرجعية.

```csharp
public string Text { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة محتوى تجريبي
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // إنشاء إدخال علامة مرجعية PDF
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "Section 1"; // Demonstrating Text property usage
            entry.Destination = worksheet.Cells["A1"];
            entry.IsOpen = true;
            
            // تعيين خيارات الحفظ مع العلامة المرجعية
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.Bookmark = entry;
            
            // حفظ دفتر العمل مع العلامة المرجعية
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF with bookmark created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


