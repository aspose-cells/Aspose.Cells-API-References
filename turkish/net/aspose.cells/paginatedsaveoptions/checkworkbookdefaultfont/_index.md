---
title: "PaginatedSaveOptions.CheckWorkbookDefaultFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdfimage içinde blok olarak görünebilirler. Bu özelliği true olarak ayarlayarak, bu karakterleri göstermek için önce çalışma kitabının varsayılan yazı tipini kullanmayı deneyin"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/
---
## PaginatedSaveOptions.CheckWorkbookDefaultFont property

Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf, görüntüde blok olarak görünebilirler. Bu değeri true olarak ayarlayın, böylece önce çalışma kitabının varsayılan yazı tipini kullanarak bu karakterleri göstermeye çalışır.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Açıklamalar

Varsayılan true'dur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Test Content");
            
            // PDF kaydetme seçeneklerini yapılandırın
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CheckWorkbookDefaultFont = false;
            
            // PDF'ye kaydet
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF saved with CheckWorkbookDefaultFont set to false");
        }
    }
}
```

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


