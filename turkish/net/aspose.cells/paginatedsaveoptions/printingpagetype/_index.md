---
title: "PaginatedSaveOptions.PrintingPageType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Hangi sayfaların yazdırılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/printingpagetype/
---
## PaginatedSaveOptions.PrintingPageType property

Hangi sayfaların yazdırılmayacağını gösterir.

```csharp
public PrintingPageType PrintingPageType { get; set; }
```

### Açıklamalar

Eğer sayfadaki içerik seyrekse, çıktı pdf dosyasında tamamen boş bazı sayfalar olacaktır. Bu boş sayfaları istemiyorsanız, bu seçeneği kullanarak onları atlayabilirsiniz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPrintingPageTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Örnek veri ekleyin
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123);
            ws.Cells["A3"].PutValue(456);
            
            // Boş çalışma sayfası oluştur
            Worksheet blankWs = wb.Worksheets.Add("BlankSheet");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Boş sayfaları yok sayarak kaydet
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            wb.Save("output_ignore_blank_page.pdf", pdfSaveOptions);
            
            // Boş sayfaları ve yalnızca stil içeren sayfaları yok sayarak kaydet
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;
            wb.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PrintingPageType](../../printingpagetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


