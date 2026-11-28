---
title: "Enum JsonExportHyperlinkType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Json.JsonExportHyperlinkType enum. Hipermetin bağlantılarını json'a nasıl dışa aktarılacağını temsil eder"
type: docs
url: /tr/net/aspose.cells.json/jsonexporthyperlinktype/
---
## JsonExportHyperlinkType enumeration

Hipermetin bağlantılarını json'a dışa aktarma tipini temsil eder.

```csharp
public enum JsonExportHyperlinkType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DisplayString | `0` | Görüntüleme dizesini dışa aktar |
| Address | `1` | URL'yi dışa aktar |
| HtmlString | `2` | HTML dizesi olarak dışa aktar |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonExportHyperlinkTypeDemo
    {
        public static void JsonExportHyperlinkTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hipermetin bağlantılarıyla bazı örnek veriler ekle
            worksheet.Cells["A1"].PutValue("Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.google.com");

            worksheet.Cells["A2"].PutValue("Aspose");
            worksheet.Hyperlinks.Add("A2", 1, 1, "http://www.aspose.com");

            // JsonSaveOptions oluştur ve ExportHyperlinkType'ı ayarla
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.DisplayString;

            // Çalışma kitabını JSON formatında kaydet
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksDisplayString.json", saveOptions);

            // ExportHyperlinkType'ı Address olarak değiştirin ve tekrar kaydedin
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.Address;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksAddress.json", saveOptions);

            // ExportHyperlinkType'ı HtmlString olarak değiştirin ve tekrar kaydedin
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksHtmlString.json", saveOptions);

            Console.WriteLine("Workbooks saved with different hyperlink export types.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Json](../../aspose.cells.json/)
* assembly [Aspose.Cells](../../)


