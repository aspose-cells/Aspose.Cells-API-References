---
title: "PdfConverter sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.PdfConverter sınıfı. Şablon dosyasını pdf'ye dönüştürmek için dönüştürücü"
type: docs
url: /tr/net/aspose.cells.lowcode/pdfconverter/
---
## PdfConverter class

Şablon dosyasını pdf'ye dönüştürmek için dönüştürücü.

```csharp
public class PdfConverter
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Şablon dosyasını pdf'ye dönüştürür |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process_1)(string, string) | Verilen şablon dosyasını pdf'ye dönüştürür. |

### Örnekler

```csharp
using System;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassPdfConverterDemo
    {
        public static void Run()
        {
            // PdfConverter'ı şablon ve çıktı yolları ile başlatın
            PdfConverter.Process("template.xlsx", "res.pdf");
            
            Console.WriteLine("PDF conversion completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


