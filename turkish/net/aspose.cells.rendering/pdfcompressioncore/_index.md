---
title: "Enum PdfCompressionCore"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.PdfCompressionCore enum. Görüntüler hariç PDF dosyasındaki tüm içeriğe uygulanan bir sıkıştırma türünü belirtir."
type: docs
url: /tr/net/aspose.cells.rendering/pdfcompressioncore/
---
## PdfCompressionCore enumeration

Görüntüler dışındaki PDF dosyasındaki tüm içeriğe uygulanan bir sıkıştırma türünü belirtir.

```csharp
public enum PdfCompressionCore
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Yok |
| Rle | `1` | Rle |
| Lzw | `2` | Lzw |
| Flate | `3` | Flate |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfCompressionCoreDemo
    {
        public static void PdfCompressionCoreExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose!");

            // PdfSaveOptions oluşturun ve PdfCompressionCore'ı ayarlayın
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate; // Setting the compression type to Flate

            // Çalışma kitabını belirtilen sıkıştırma ile bir PDF dosyası olarak kaydedin
            workbook.Save("PdfCompressionCoreExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file saved with specified compression.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


