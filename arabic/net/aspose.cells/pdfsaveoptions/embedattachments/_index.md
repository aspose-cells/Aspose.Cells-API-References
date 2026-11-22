---
title: "PdfSaveOptions.EmbedAttachments"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تشير إلى ما إذا كان يجب تضمين المرفق لكائنات Ole في Excel"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/embedattachments/
---
## PdfSaveOptions.EmbedAttachments property

يشير إلى ما إذا كان يجب تضمين مرفق لكائنات Ole في Excel.

```csharp
public bool EmbedAttachments { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false. يجب أن تكون القيمة false عندما يتم تعيين الامتثال لـ PDF/A أو يتم تمكين تشفير pdf.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
using System.IO;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedAttachmentsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF with Embedded Attachments Example");

            // أنشئ ملفًا تجريبيًا لتضمينه
            string sampleFile = "sample.docx";
            File.WriteAllText(sampleFile, "This is a sample document");

            // أضف مرفقًا (كائن OLE) إلى ورقة العمل
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(sampleFile));
            worksheet.OleObjects[oleIndex].FileFormatType = FileFormatType.Docx;
            worksheet.OleObjects[oleIndex].DisplayAsIcon = true;

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // عيّن خاصية EmbedAttachments إلى true
            pdfSaveOptions.EmbedAttachments = true;

            // احفظ المصنف كملف PDF مع مرفقات مضمَّنة
            workbook.Save("PdfWithEmbeddedAttachments.pdf", pdfSaveOptions);

            // تنظيف
            File.Delete(sampleFile);
        }
    }
}
```

### انظر أيضًا

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


