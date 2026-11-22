---
title: "تعداد PdfCustomPropertiesExport"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Rendering.PdfCustomPropertiesExport. يحدد الطريقة التي يتم بها تصدير CustomDocumentPropertyCollection إلى ملف PDF"
type: docs
url: /ar/net/aspose.cells.rendering/pdfcustompropertiesexport/
---
## PdfCustomPropertiesExport enumeration

يحدد الطريقة التي يتم بها تصدير [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) إلى ملف PDF.

```csharp
public enum PdfCustomPropertiesExport
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | لم يتم تصدير أي خصائص مخصصة. |
| Standard | `1` | يتم تصدير الخصائص المخصصة كإدخالات في قاموس Info. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfCustomPropertiesExportDemo
    {
        public static void PdfCustomPropertiesExportExample()
        {
            // أنشئ مصنفًا وأضف بعض البيانات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("This is a sample document");

            // عيّن بعض الخصائص المخصصة
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("Subject", "Sample PDF Export");

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // عيّن خيار تصدير الخصائص المخصصة
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            // احفظ المصنف كملف PDF
            workbook.Save("PdfCustomPropertiesExportExample.pdf", saveOptions);

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


