---
title: "HtmlSaveOptions.WorksheetScalable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML dosyasını kaydederken çalışma sayfası yakınlaştırma seviyesine göre HTML'yi yakınlaştırıp uzaklaştırıp uzaklaştırmadığını gösterir, varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/worksheetscalable/
---
## HtmlSaveOptions.WorksheetScalable property

Dosya HTML olarak kaydedilirken çalışma sayfası yakınlaştırma düzeyiyle HTML'yi yakınlaştırıp uzaklaştırmayacağını gösterir, varsayılan değer false.

```csharp
public bool WorksheetScalable { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWorksheetScalableDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // WorksheetScalable özelliği ile HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WorksheetScalable = true;
            
            // Çalışma kitabını HTML seçenekleriyle kaydet
            string outputPath = "output.html";
            workbook.Save(outputPath, options);
            
            // Çıktının ölçekleme stilini içerdiğini doğrulayın
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains scaling: " + htmlContent.Contains("transform: scale"));
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


