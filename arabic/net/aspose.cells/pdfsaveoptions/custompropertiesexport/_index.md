---
title: "PdfSaveOptions.CustomPropertiesExport"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعين قيمة تحدد طريقة تصدير CustomDocumentPropertyCollection إلى ملف PDF. القيمة الافتراضية هي None"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/custompropertiesexport/
---
## PdfSaveOptions.CustomPropertiesExport property

تحصل أو تعين قيمة تحدد طريقة تصدير [`CustomDocumentPropertyCollection`](../../../aspose.cells.properties/customdocumentpropertycollection/) إلى ملف PDF. القيمة الافتراضية هي None.

```csharp
public PdfCustomPropertiesExport CustomPropertiesExport { get; set; }
```

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCustomPropertiesExportDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("Sample PDF Export");

            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Subject", "Aspose.Cells Example");

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            workbook.Save("PdfCustomPropertiesExportDemo.pdf", saveOptions);
        }
    }
}
```

### انظر أيضًا

* enum [PdfCustomPropertiesExport](../../../aspose.cells.rendering/pdfcustompropertiesexport/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


