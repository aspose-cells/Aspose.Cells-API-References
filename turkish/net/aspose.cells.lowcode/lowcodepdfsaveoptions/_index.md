---
title: "Sınıf LowCodePdfSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.LowCodePdfSaveOptions sınıfı. PDF'yi düşük kod yöntemiyle kaydetmek için seçenekler"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodepdfsaveoptions/
---
## LowCodePdfSaveOptions class

Düşük kodlu bir şekilde PDF kaydetme seçenekleri.

```csharp
public class LowCodePdfSaveOptions : LowCodeSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LowCodePdfSaveOptions](lowcodepdfsaveoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır ve ayarlar. Bu özelliği null veya boş dize dışındaki bir değerle ayarladığınızda, [`OutputStream`](../lowcodesaveoptions/outputstream/) yok sayılacaktır. ([`LowCodeSaveOptions`](../lowcodesaveoptions/) sınıfından devralınmıştır.) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Oluşturulan verileri yazmak için akışı alır ve ayarlar. Bu özelliği null dışındaki bir değerle ayarladığınızda, [`OutputFile`](../lowcodesaveoptions/outputfile/) yok sayılacaktır. ([`LowCodeSaveOptions`](../lowcodesaveoptions/) sınıfından devralınmıştır.) |
| [PdfOptions](../../aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/) { get; set; } | Pdf dosyasını kaydetmek için seçenekler. |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/) { get; set; } | Çıktı için kaydetme formatı. Pdf'ye dönüştürme için yalnızca Pdf olabilir. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodePdfSaveOptionsDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Compliance = PdfCompliance.PdfA1b;

            // Düşük kodlu PDF kaydetme seçeneklerini oluşturun
            LowCodePdfSaveOptions lowCodePdfOptions = new LowCodePdfSaveOptions()
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfOptions
            };

            // Düşük kodlu seçenekleri kullanarak kaydedin
            workbook.Save(lowCodePdfOptions.OutputFile, lowCodePdfOptions.PdfOptions);

            Console.WriteLine("File saved successfully with LowCodePdfSaveOptions");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


