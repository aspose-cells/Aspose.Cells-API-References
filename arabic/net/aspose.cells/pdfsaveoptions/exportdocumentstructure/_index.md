---
title: "PdfSaveOptions.ExportDocumentStructure"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تشير إلى ما إذا كان سيتم تصدير بنية المستند"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/exportdocumentstructure/
---
## PdfSaveOptions.ExportDocumentStructure property

يشير إلى ما إذا كان يجب تصدير بنية المستند.

```csharp
public bool ExportDocumentStructure { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyExportDocumentStructureDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // عيّن ExportDocumentStructure إلى true للاحتفاظ ببنية المستند
            pdfSaveOptions.ExportDocumentStructure = true;
            
            // احسب الصيغ قبل الحفظ
            workbook.CalculateFormula();

            // احفظ المصنف كملف PDF باستخدام الخيارات المحددة
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with document structure exported.");
        }
    }
}
```

### انظر أيضًا

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


