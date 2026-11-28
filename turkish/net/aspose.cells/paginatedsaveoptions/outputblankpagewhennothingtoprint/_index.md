---
title: "PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/
---
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property

Yazdırılacak bir şey olmadığında boş bir sayfa çıktısı verilip verilmeyeceğini gösterir.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Açıklamalar

Varsayılan true'dur.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekleyin ve gizleyin (yazdırılacak bir şey olmadığını taklit eder)
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.IsVisible = false;

            // OutputBlankPageWhenNothingToPrint = false ile PDF kaydetme seçeneklerini ayarlayın
            PdfSaveOptions options = new PdfSaveOptions
            {
                OutputBlankPageWhenNothingToPrint = false
            };

            // PDF'ye kaydedin - boş sayfa oluşturulmamalıdır
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputNoBlankPage.pdf");
            workbook.Save(outputPath, options);

            // Seçeneği true olarak değiştirin
            options.OutputBlankPageWhenNothingToPrint = true;

            // Tekrar kaydet - boş bir sayfa oluşturulmalıdır
            outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputWithBlankPage.pdf");
            workbook.Save(outputPath, options);
        }
    }
}
```

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


