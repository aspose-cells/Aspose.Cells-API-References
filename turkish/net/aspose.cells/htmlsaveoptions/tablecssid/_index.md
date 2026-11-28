---
title: "HtmlSaveOptions.TableCssId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. trcoltd gibi tip css adının önekini alır ve ayarlar; bu önek, belirli TableCssId özniteliğine sahip tablo öğesinde bulunur. Varsayılan değer "
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/tablecssid/
---
## HtmlSaveOptions.TableCssId property

tr, col, td vb. gibi tip css adının önekini alır ve ayarlar; bu önek, belirli TableCssId özniteliğine sahip tablo öğesinde bulunur. Varsayılan değer "".

```csharp
public string TableCssId { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyTableCssIdDemo
    {
        public static void Run()
        {
            // Test verileriyle örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // TableCssId ile HTML kaydetme seçeneklerini yapılandırın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.TableCssId = "custom-table-style";
            
            // Çalışma kitabını HTML seçenekleriyle kaydet
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with TableCssId: " + saveOptions.TableCssId);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


