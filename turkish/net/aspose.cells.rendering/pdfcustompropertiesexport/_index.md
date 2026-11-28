---
title: "Enum PdfCustomPropertiesExport"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.PdfCustomPropertiesExport enum. CustomDocumentPropertyCollection öğelerinin PDF dosyasına nasıl dışa aktarıldığını belirtir."
type: docs
url: /tr/net/aspose.cells.rendering/pdfcustompropertiesexport/
---
## PdfCustomPropertiesExport enumeration

`[`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/)` öğelerinin PDF dosyasına nasıl dışa aktarıldığını belirtir.

```csharp
public enum PdfCustomPropertiesExport
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Hiçbir özel özellik dışa aktarılmaz. |
| Standard | `1` | Özel özellikler, Info sözlüğündeki girişler olarak dışa aktarılır. |

### Örnekler

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
            // Bir çalışma kitabı oluşturun ve bazı veriler ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("This is a sample document");

            // Bazı özel özellikleri ayarlayın
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("Subject", "Sample PDF Export");

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Özel özellik dışa aktarma seçeneğini ayarlayın
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            // Çalışma kitabını PDF olarak kaydedin
            workbook.Save("PdfCustomPropertiesExportExample.pdf", saveOptions);

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


