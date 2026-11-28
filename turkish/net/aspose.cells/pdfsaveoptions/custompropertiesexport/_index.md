---
title: "PdfSaveOptions.CustomPropertiesExport"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. CustomDocumentPropertyCollection'ın PDF dosyasına nasıl dışa aktarılacağını belirleyen bir değeri alır veya ayarlar. Varsayılan değer None'dur"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/custompropertiesexport/
---
## PdfSaveOptions.CustomPropertiesExport property

[`CustomDocumentPropertyCollection`](../../../aspose.cells.properties/customdocumentpropertycollection/) PDF dosyasına nasıl dışa aktarılacağını belirleyen bir değeri alır veya ayarlar. Varsayılan değer None'dur.

```csharp
public PdfCustomPropertiesExport CustomPropertiesExport { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* enum [PdfCustomPropertiesExport](../../../aspose.cells.rendering/pdfcustompropertiesexport/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


