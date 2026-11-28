---
title: "HtmlSaveOptions.ExportPageFooters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportpagefooters/
---
## HtmlSaveOptions.ExportPageFooters property

Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir.

```csharp
public bool ExportPageFooters { get; set; }
```

### Açıklamalar

Yalnızca [`SaveAsSingleFile`](../saveassinglefile/) True olduğunda çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageFootersDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Çıktıya sayfa altbilgilerini eklemek için ExportPageFooters'ı true olarak ayarlayın
            saveOptions.ExportPageFooters = true;
            
            // Diğer gerekli seçenekleri ayarlayın
            saveOptions.ExportPageHeaders = true;
            
            // Çalışma kitabını HTML olarak kaydedin
            workbook.Save("HtmlWithPageFooters.html", saveOptions);
            
            Console.WriteLine("HTML file with page footers exported successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


