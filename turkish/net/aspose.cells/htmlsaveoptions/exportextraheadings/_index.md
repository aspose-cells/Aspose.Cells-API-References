---
title: "HtmlSaveOptions.ExportExtraHeadings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Metin uzunluğu maksimum gösterim sütunundan uzun olduğunda ek başlıkların dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. HTML dosyasını Excel'e içe aktarmak istiyorsanız lütfen varsayılan değeri koruyun."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportextraheadings/
---
## HtmlSaveOptions.ExportExtraHeadings property

Metin uzunluğu maksimum görüntüleme sütunundan daha uzun olduğunda ekstra başlıkların dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. HTML dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

```csharp
public bool ExportExtraHeadings { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportExtraHeadingsDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ve ek başlıklar ekle
            worksheet.Cells["A1"].PutValue("Main Heading");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");
            
            // Ek başlıkları ayarla (satırlar ve sütunlar)
            worksheet.Cells["Z1"].PutValue("Extra Column Heading");
            worksheet.Cells["A100"].PutValue("Extra Row Heading");

            // ExportExtraHeadings ile HTML kaydetme seçeneklerini yapılandır
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportHeadings = true;
            saveOptions.ExportExtraHeadings = true;

            // HTML olarak kaydet
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML exported with extra headings.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


