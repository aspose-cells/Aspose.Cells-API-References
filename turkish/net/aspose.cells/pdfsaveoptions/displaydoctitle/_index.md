---
title: "PdfSaveOptions.DisplayDocTitle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. Windows başlık çubuğunun belge başlığını gösterip göstermeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/displaydoctitle/
---
## PdfSaveOptions.DisplayDocTitle property

Pencerenin başlık çubuğunun belge başlığını gösterip göstermeyeceğini gösterir.

```csharp
public bool DisplayDocTitle { get; set; }
```

### Açıklamalar

False ise, başlık çubuğu bunun yerine PDF dosyasının adını göstermelidir. Varsayılan değer false'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyDisplayDocTitleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF DisplayDocTitle Example");

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // DisplayDocTitle özelliğini true olarak ayarlayın
            pdfSaveOptions.DisplayDocTitle = true;

            // Çalışma kitabını PDF olarak kaydedin
            workbook.Save("PdfDisplayDocTitleDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


