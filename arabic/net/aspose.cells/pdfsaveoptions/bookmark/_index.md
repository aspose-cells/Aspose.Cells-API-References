---
title: "PdfSaveOptions.Bookmark"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تحصل وتعيّن كائن PdfBookmarkEntry"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/bookmark/
---
## PdfSaveOptions.Bookmark property

تحصل وتعيّن كائن [`PdfBookmarkEntry`](../../../aspose.cells.rendering/pdfbookmarkentry/).

```csharp
public PdfBookmarkEntry Bookmark { get; set; }
```

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyBookmarkDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ثلاث أوراق عمل
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            Worksheet sheet3 = workbook.Worksheets.Add("Sheet3");

            // عيّن القيم في الخلايا التي ستكون وجهات الإشارات المرجعية
            sheet1.Cells["A1"].Value = "Sheet1 Content";
            sheet2.Cells["A1"].Value = "Sheet2 Content";
            sheet3.Cells["A1"].Value = "Sheet3 Content";

            // أنشئ إشارة مرجعية جذرية
            PdfBookmarkEntry rootBookmark = new PdfBookmarkEntry
            {
                Text = "Root",
                Destination = sheet1.Cells["A1"],
                IsOpen = true
            };

            // أنشئ إشارات مرجعية فرعية
            PdfBookmarkEntry subBookmark1 = new PdfBookmarkEntry
            {
                Text = "Sheet2",
                Destination = sheet2.Cells["A1"]
            };

            PdfBookmarkEntry subBookmark2 = new PdfBookmarkEntry
            {
                Text = "Sheet3",
                Destination = sheet3.Cells["A1"]
            };

            // أضف إشارات مرجعية فرعية إلى الجذر
            rootBookmark.SubEntry = new ArrayList { subBookmark1, subBookmark2 };

            // قم بتكوين خيارات حفظ PDF مع الإشارات المرجعية
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = rootBookmark
            };

            // احفظ إلى تدفق الذاكرة (يمكن حفظه إلى ملف في الاستخدام الفعلي)
            workbook.Save("output.pdf", options);
        }
    }
}
```

### انظر أيضًا

* class [PdfBookmarkEntry](../../../aspose.cells.rendering/pdfbookmarkentry/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


