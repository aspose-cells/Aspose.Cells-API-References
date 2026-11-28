---
title: "Enum HtmlCrossType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HtmlCrossType enum. HTML çapraz dize tipinin beş türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enumeration

HTML çapraz dize beş türünü temsil eder.

```csharp
public enum HtmlCrossType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | MS Excel gibi göster, sonraki hücreye bağlıdır. Eğer sonraki hücre null ise, dize çaprazlaşır, aksi takdirde kesilir |
| MSExport | `1` | Dizeyi MS Excel gibi HTML dışa aktararak göster. |
| Cross | `2` | HTML çapraz dizesini göster, büyük HTML dosyaları oluştururken bu performans, değeri Default veya FitToCell olarak ayarlamaktan on kat daha hızlı olacaktır. |
| CrossHideRight | `3` | HTML çapraz dizesini göster ve metinler üst üste geldiğinde sağdaki dizeyi gizle. |
| FitToCell | `4` | Sadece hücrenin genişliği içinde dizeyi göster. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHtmlCrossTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);
            
            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Çapraz tipini MSExport olarak ayarla
            options.HtmlCrossStringType = HtmlCrossType.MSExport;
            
            // Çalışma kitabını HTML seçenekleriyle kaydet
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with HtmlCrossType.MSExport");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


