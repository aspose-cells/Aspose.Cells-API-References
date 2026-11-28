---
title: "Enum HtmlLinkTargetType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HtmlLinkTargetType enum. HTML etiketindeki target özniteliğinin tipini temsil eder"
type: docs
url: /tr/net/aspose.cells/htmllinktargettype/
---
## HtmlLinkTargetType enumeration

HTML  etiketindeki hedef özniteliğin türünü temsil eder.

```csharp
public enum HtmlLinkTargetType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Blank | `0` | Bağlantılı belgeyi yeni bir pencere ya da sekmede açar |
| Parent | `1` | Bağlantılı belgeyi üst çerçevede açar |
| Self | `2` | Bağlantılı belgeyi tıklandığı aynı çerçevede açar (bu varsayılandır) |
| Top | `3` | Bağlantılı belgeyi pencerenin tam gövdesinde açar |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLinkTargetTypeDemo
    {
        public static void HtmlLinkTargetTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Click here to visit Aspose");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // HtmlSaveOptions oluştur ve LinkTargetType'ı ayarla
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank; // Opens the link in a new window or tab

            // Çalışma kitabını HTML formatında kaydedin
            workbook.Save("HtmlLinkTargetTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with link target type set to '_blank'.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


