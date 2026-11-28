---
title: "HtmlSaveOptions.ExportBogusRowData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Sahte alt satır verilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız lütfen varsayılan değeri koruyun."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportbogusrowdata/
---
## HtmlSaveOptions.ExportBogusRowData property

Alt satırdaki sahte verilerin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

```csharp
public bool ExportBogusRowData { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportBogusRowDataDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            
            // İlk olarak sahte satır verisi olmadan dışa aktarın
            saveOptions.ExportBogusRowData = false;
            workbook.Save("output_without_bogus.html", saveOptions);
            
            // Ardından sahte satır verisiyle dışa aktarın
            saveOptions.ExportBogusRowData = true;
            workbook.Save("output_with_bogus.html", saveOptions);

            // Sonuçları görüntüleyin
            Console.WriteLine("HTML files created successfully.");
            Console.WriteLine("Check output_without_bogus.html and output_with_bogus.html to see the difference.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


