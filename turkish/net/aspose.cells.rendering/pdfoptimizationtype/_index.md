---
title: "Enum PdfOptimizationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.PdfOptimizationType enum. Bir optimizasyon türünü belirtir."
type: docs
url: /tr/net/aspose.cells.rendering/pdfoptimizationtype/
---
## PdfOptimizationType enumeration

Bir optimizasyon türünü belirtir.

```csharp
public enum PdfOptimizationType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Standard | `0` | Yüksek baskı kalitesi |
| MinimumSize | `1` | Dosya boyutu, baskı kalitesinden daha önemlidir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfOptimizationTypeDemo
    {
        public static void PdfOptimizationTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // PdfSaveOptions oluşturun ve optimizasyon türünü ayarlayın.
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Çalışma kitabını belirtilen optimizasyon türüyle PDF olarak kaydedin.
            workbook.Save("OptimizedOutput.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with optimization type: MinimumSize");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


