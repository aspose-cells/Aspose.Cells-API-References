---
title: "Enum PdfFontEncoding"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.PdfFontEncoding enum. PDF gömülü yazı tipi kodlamasını temsil eder"
type: docs
url: /tr/net/aspose.cells.rendering/pdffontencoding/
---
## PdfFontEncoding enumeration

PDF gömülü yazı tipi kodlamasını temsil eder.

```csharp
public enum PdfFontEncoding
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Identity | `0` | PDF'deki tüm gömülü yazı tipleri için Identity-H kodlamasının kullanılmasını temsil eder. |
| AnsiPrefer | `1` | Karakterleri 32-127 aralığında olan TrueType yazı tipleri için WinAnsiEncoding kullanılmasını tercih eder, aksi takdirde PDF'deki gömülü yazı tipleri için Identity-H kodlaması kullanılacaktır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfFontEncodingDemo
    {
        public static void PdfFontEncodingExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");

            // PdfSaveOptions oluşturun ve FontEncoding özelliğini ayarlayın
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;

            // Çalışma kitabını PDF dosyası olarak kaydedin
            workbook.Save("PdfFontEncodingExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file created successfully with specified font encoding.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


