---
title: "PdfBookmarkEntry.Destination"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfBookmarkEntry. الخلية التي يرتبط بها رابط العلامة المرجعية"
type: docs
url: /ar/net/aspose.cells.rendering/pdfbookmarkentry/destination/
---
## PdfBookmarkEntry.Destination property

الخلية التي يرتبط بها رابط الإشارة المرجعية

```csharp
public Cell Destination { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyDestinationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة محتوى تجريبي
            worksheet.Cells["A1"].PutValue("Bookmark Destination");
            
            // تكوين خيارات حفظ PDF مع العلامة المرجعية
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "Sample Bookmark";
            entry.Destination = worksheet.Cells["A1"]; // Demonstrate Destination property
            entry.IsOpen = true;
            
            pdfSaveOptions.Bookmark = entry;
            
            // حفظ ملف PDF
            workbook.Save("PdfBookmarkEntryPropertyDestinationDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../../aspose.cells/cell/)
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


