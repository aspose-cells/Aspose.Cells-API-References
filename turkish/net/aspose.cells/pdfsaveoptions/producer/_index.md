---
title: "PdfSaveOptions.Producer"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. Oluşturulan pdf belgesinin üreticisini alır ve ayarlar."
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/producer/
---
## PdfSaveOptions.Producer property

Oluşturulan PDF belgesinin üreticisini alır ve ayarlar.

```csharp
public string Producer { get; set; }
```

### Açıklamalar

Değer null ise veya geçerli bir LICENSE ayarlanmamışsa, Aspose.Cells vVERSION dizesi kullanılacaktır.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyProducerDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına erişin ve örnek veri ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Producer Property Demo");

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Producer özelliğini ayarla
            pdfSaveOptions.Producer = "Aspose.Cells for .NET";
            
            // Bellek akışına kaydet
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Producer'ın ayarlandığını doğrula
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine(content.Contains("/Producer (Aspose.Cells for .NET)") 
                        ? "Producer property set successfully" 
                        : "Failed to set Producer property");
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


