---
title: "الفئة PdfBookmarkEntry"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.PdfBookmarkEntry. PdfBookmarkEntry هو إدخال في إشارة مرجعية PDF. إذا كانت خاصية Text للكائن الحالي فارغة أو null فسيتم إخفاء الكائن الحالي وسيتم إدراج العناصر الفرعية في المستوى الحالي"
type: docs
url: /ar/net/aspose.cells.rendering/pdfbookmarkentry/
---
## PdfBookmarkEntry class

PdfBookmarkEntry هو إدخال في إشارة مرجعية PDF. إذا كانت الخاصية Text للنسخة الحالية فارغة أو "", سيتم إخفاء النسخة الحالية وسيتم إدراج العناصر الفرعية في المستوى الحالي.

```csharp
public class PdfBookmarkEntry
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PdfBookmarkEntry](pdfbookmarkentry/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Destination](../../aspose.cells.rendering/pdfbookmarkentry/destination/) { get; set; } | الخلية التي يرتبط بها رابط الإشارة المرجعية |
| [DestinationName](../../aspose.cells.rendering/pdfbookmarkentry/destinationname/) { get; set; } | يحصل أو يعيّن اسم الوجهة. |
| [IsCollapse](../../aspose.cells.rendering/pdfbookmarkentry/iscollapse/) { get; set; } | عند تكون هذه الخاصية true، سيُطوى bookmarkentry، وإلا سيتوسع. |
| [IsOpen](../../aspose.cells.rendering/pdfbookmarkentry/isopen/) { get; set; } | عند تكون هذه الخاصية true، سيتوسع bookmarkentry، وإلا سيُطوى. |
| [SubEntry](../../aspose.cells.rendering/pdfbookmarkentry/subentry/) { get; set; } | SubEntry لإشارة مرجعية. |
| [Text](../../aspose.cells.rendering/pdfbookmarkentry/text/) { get; set; } | عنوان إشارة مرجعية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Collections;

    public class PdfBookmarkEntryDemo
    {
        public static void PdfBookmarkEntryExample()
        {
            // إنشاء مصنف جديد وإضافة أوراق عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // الحصول على الخلايا من كل ورقة عمل
            Cell cellInPage1 = workbook.Worksheets[0].Cells["A1"];
            Cell cellInPage2 = workbook.Worksheets[1].Cells["A1"];
            Cell cellInPage3 = workbook.Worksheets[2].Cells["A1"];

            // وضع القيم في الخلايا
            cellInPage1.PutValue("page1");
            cellInPage2.PutValue("page2");
            cellInPage3.PutValue("page3");

            // إنشاء PdfBookmarkEntry الجذر
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry
            {
                Text = "root",  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
                Destination = cellInPage1,
                SubEntry = new ArrayList(),
                IsOpen = false
            };

            // إنشاء PdfBookmarkEntries فرعية
            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry
            {
                Text = "section1",
                Destination = cellInPage2
            };

            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry
            {
                Text = "section2",
                Destination = cellInPage3
            };

            // إضافة إدخالات فرعية إلى الإدخال الجذر
            pbeRoot.SubEntry.Add(subPbe1);
            pbeRoot.SubEntry.Add(subPbe2);

            // إنشاء PdfSaveOptions وتعيين الإشارة المرجعية
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Bookmark = pbeRoot
            };

            // حفظ المصنف كملف PDF مع الإشارات المرجعية
            workbook.Save("output_bookmark.pdf", saveOptions);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


