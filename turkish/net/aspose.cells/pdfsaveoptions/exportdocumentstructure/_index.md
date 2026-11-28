---
title: "PdfSaveOptions.ExportDocumentStructure"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. Belge yapısının dışa aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/exportdocumentstructure/
---
## PdfSaveOptions.ExportDocumentStructure property

Belge yapısını dışa aktarılıp aktarılmayacağını gösterir.

```csharp
public bool ExportDocumentStructure { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyExportDocumentStructureDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Belge yapısını korumak için ExportDocumentStructure'ı true olarak ayarlayın
            pdfSaveOptions.ExportDocumentStructure = true;
            
            // Kaydetmeden önce formülleri hesaplayın
            workbook.CalculateFormula();

            // Çalışma kitabını belirtilen seçeneklerle PDF olarak kaydet
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with document structure exported.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


