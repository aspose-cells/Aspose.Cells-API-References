---
title: "PdfSaveOptions.CalculateFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. PDF dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/calculateformula/
---
## PdfSaveOptions.CalculateFormula property

PDF dosyasını kaydetmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir.

```csharp
public bool CalculateFormula { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Örnek veri ve formüller içeren bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Değerleri ve formülleri ayarla.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Formül hesaplamalı PDF kaydetme seçenekleri oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.CalculateFormula = true;

            // Bellek akışına kaydet
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Akış konumunu sıfırla ve içeriği doğrula
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine("PDF contains formula results: " + content.Contains("30"));
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


