---
title: "PdfBookmarkEntry.DestinationName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfBookmarkEntry. الحصول على اسم الوجهة أو تعيينه"
type: docs
url: /ar/net/aspose.cells.rendering/pdfbookmarkentry/destinationname/
---
## PdfBookmarkEntry.DestinationName property

يحصل أو يعيّن اسم الوجهة.

```csharp
public string DestinationName { get; set; }
```

### ملاحظات

إذا تم تعيين اسم الوجهة، سيتم تعريف الوجهة كوجهة مسماة بهذا الاسم.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfBookmarkEntryPropertyDestinationNameDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة محتوى تجريبي إلى الخلايا
            worksheet.Cells["A1"].PutValue("Primary Content Section");
            worksheet.Cells["A2"].PutValue("Secondary Content Section");

            // إنشاء إدخال علامة مرجعية PDF رئيسي
            PdfBookmarkEntry mainEntry = new PdfBookmarkEntry
            {
                Text = "Main Section",
                Destination = worksheet.Cells["A1"],
                IsOpen = true
            };

            // عرض قراءة قيمة DestinationName الأولية (null)
            Console.WriteLine($"Initial DestinationName: {mainEntry.DestinationName ?? "null"}");

            // تعيين اسم وجهة مخصص للإدخال الرئيسي
            mainEntry.DestinationName = "PrimaryDestination";
            Console.WriteLine($"Updated DestinationName: {mainEntry.DestinationName}");

            // إنشاء إدخال علامة مرجعية فرعية
            PdfBookmarkEntry subEntry = new PdfBookmarkEntry
            {
                Text = "Sub Section",
                Destination = worksheet.Cells["A2"],
                DestinationName = "SecondaryDestination"
            };

            // إضافة إدخال فرعي إلى العلامة المرجعية الرئيسية
            mainEntry.SubEntry = new System.Collections.ArrayList { subEntry };

            // تكوين خيارات حفظ PDF مع بنية العلامات المرجعية
            PdfSaveOptions pdfOptions = new PdfSaveOptions
            {
                Bookmark = mainEntry
            };

            // حفظ المصنف مع علامات PDF المرجعية
            workbook.Save("PdfBookmarkDestinationDemo.pdf", pdfOptions);

            Console.WriteLine("PDF created with custom bookmark destinations.");
        }
    }
}
```

### انظر أيضًا

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


