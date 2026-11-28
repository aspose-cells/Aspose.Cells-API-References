---
title: "PdfSaveOptions.OptimizationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. PDF optimizasyon türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/optimizationtype/
---
## PdfSaveOptions.OptimizationType property

PDF optimizasyon türünü alır ve ayarlar.

```csharp
public PdfOptimizationType OptimizationType { get; set; }
```

### Açıklamalar

Varsayılan değer Standard'dır

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyOptimizationTypeDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Optimization Example");

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // OptimizationType özelliğini gösterin
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Çalışma kitabını optimizasyon ayarlarıyla kaydedin
            workbook.Save("OptimizedPdf.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PdfOptimizationType](../../../aspose.cells.rendering/pdfoptimizationtype/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


