---
title: "PaginatedSaveOptions.IgnoreError"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Oluşturma sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir. Hata şekil, resim, grafik oluşturma vb. hatalar olabilir"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

Renderleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir. Hata şekil, görüntü, grafik renderlemesinde vb. bir hata olabilir.

```csharp
public bool IgnoreError { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Olası biçimlendirme hataları içeren bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            
            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Herhangi bir dönüşüm hatasını atlamak için IgnoreError'i true olarak ayarlayın
            options.IgnoreError = true;
            
            // Çalışma kitabını PDF olarak kaydedin
            workbook.Save("PaginatedSaveWithIgnoreError.pdf", options);
            
            Console.WriteLine("PDF saved with IgnoreError enabled.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


