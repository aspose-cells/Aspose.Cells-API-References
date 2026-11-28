---
title: "PdfSaveOptions.PdfCompression"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. Sıkıştırma algoritmasını belirtir"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/pdfcompression/
---
## PdfSaveOptions.PdfCompression property

Sıkıştırma algoritmasını belirtin

```csharp
public PdfCompressionCore PdfCompression { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyPdfCompressionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş ve örnek veri ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample PDF Compression Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfCompression property usage");
            
            // Flate sıkıştırmalı PDF kaydetme seçenekleri oluşturun
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PdfCompression = PdfCompressionCore.Flate;
            
            // Çalışma kitabını sıkıştırmalı PDF olarak kaydedin
            workbook.Save("output_with_flate_compression.pdf", saveOptions);
            
            // Karşılaştırma için sıkıştırma olmadan tekrar kaydedin
            saveOptions.PdfCompression = PdfCompressionCore.None;
            workbook.Save("output_without_compression.pdf", saveOptions);
            
            Console.WriteLine("PDF files created successfully with different compression settings.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PdfCompressionCore](../../../aspose.cells.rendering/pdfcompressioncore/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


