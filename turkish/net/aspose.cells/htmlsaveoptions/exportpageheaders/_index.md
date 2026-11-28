---
title: "HtmlSaveOptions.ExportPageHeaders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportpageheaders/
---
## HtmlSaveOptions.ExportPageHeaders property

Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir.

```csharp
public bool ExportPageHeaders { get; set; }
```

### Açıklamalar

Yalnızca [`SaveAsSingleFile`](../saveassinglefile/) True olduğunda çalışır.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageHeadersDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sayfa üstbilgisini ayarlayın
            worksheet.PageSetup.SetHeader(0, "Sample Header Text");
            
            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("This is a test");
            
            // HTML kaydetme seçeneklerini yapılandır
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                SaveAsSingleFile = true,
                ShowAllSheets = true,
                ExportPageHeaders = true  // This is the key property being demonstrated
            };
            
            // Çalışma kitabını HTML olarak kaydet
            string outputPath = "output_with_headers.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with page headers exported successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


