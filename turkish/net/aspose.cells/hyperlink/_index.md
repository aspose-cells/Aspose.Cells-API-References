---
title: "Hyperlink sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Hyperlink sınıfı. Bir köprüyü temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells/hyperlink/
---
## Hyperlink class

Bir köprüyi temsil eden nesneyi kapsüller.

```csharp
public class Hyperlink
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Address](../../aspose.cells/hyperlink/address/) { get; set; } | Bir köprünün adresini temsil eder. |
| [Area](../../aspose.cells/hyperlink/area/) { get; } | Köprünün aralığını alır. |
| [LinkType](../../aspose.cells/hyperlink/linktype/) { get; } | Köprü tipini alır. |
| [ScreenTip](../../aspose.cells/hyperlink/screentip/) { get; set; } | Belirtilen köprü için ScreenTip metnini döndürür veya ayarlar. |
| [TextToDisplay](../../aspose.cells/hyperlink/texttodisplay/) { get; set; } | Belirtilen köprü için görüntülenecek metni temsil eder. Varsayılan değer köprünün adresidir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Delete](../../aspose.cells/hyperlink/delete/)() | Bu köprüyü siler |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkDemo
    {
        public static void HyperlinkExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            
            // Workbook nesnesine yeni bir çalışma sayfası ekleme
            workbook.Worksheets.Add();
            
            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[0];
            
            // \"A1\" hücresine bir URL'ye köprü ekleme
            int index = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");
            
            // İndeks ile bir Köprü alınıyor
            Hyperlink hyperlink = worksheet.Hyperlinks[index];
            
            // Bu köprünün görüntüleme metnini ayarlama
            hyperlink.TextToDisplay = "Aspose";
            
            // Köprü için ScreenTip metnini ayarlama
            hyperlink.ScreenTip = "Visit Aspose Website";
            
            // Excel dosyasını kaydetme
            workbook.Save("HyperlinkExample.xlsx");
            workbook.Save("HyperlinkExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


