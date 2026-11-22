---
title: "PdfBookmarkEntry.SubEntry"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfBookmarkEntry. الإدخال الفرعي لعلامة مرجعية"
type: docs
url: /ar/net/aspose.cells.rendering/pdfbookmarkentry/subentry/
---
## PdfBookmarkEntry.SubEntry property

SubEntry لإشارة مرجعية.

```csharp
public ArrayList SubEntry { get; set; }
```

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertySubEntryDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // إنشاء إدخال علامة مرجعية جذرية
            PdfBookmarkEntry root = new PdfBookmarkEntry
            {
                Text = "Main Bookmark",
                Destination = workbook.Worksheets[0].Cells["A1"],
                SubEntry = new ArrayList(),
                IsOpen = true
            };

            // أنشئ إشارات مرجعية فرعية
            PdfBookmarkEntry sub1 = new PdfBookmarkEntry
            {
                Text = "First Section",
                Destination = workbook.Worksheets[1].Cells["A1"]
            };

            PdfBookmarkEntry sub2 = new PdfBookmarkEntry
            {
                Text = "Second Section",
                Destination = workbook.Worksheets[2].Cells["A1"],
                SubEntry = new ArrayList()
            };

            // إضافة علامة مرجعية فرعية متداخلة
            PdfBookmarkEntry subSub = new PdfBookmarkEntry
            {
                Text = "Sub-Section",
                Destination = workbook.Worksheets[2].Cells["B1"]
            };
            sub2.SubEntry.Add(subSub);

            // أضف إشارات مرجعية فرعية إلى الجذر
            root.SubEntry.Add(sub1);
            root.SubEntry.Add(sub2);

            // حفظ مع العلامات المرجعية
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = root
            };
            workbook.Save("output_with_bookmarks.pdf", options);
        }
    }
}
```

### انظر أيضًا

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


