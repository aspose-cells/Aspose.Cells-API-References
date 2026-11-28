---
title: "Enum DynamicFilterType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DynamicFilterType enum. Dinamik filtre türü"
type: docs
url: /tr/net/aspose.cells/dynamicfiltertype/
---
## DynamicFilterType enumeration

Dinamik filtre türü.

```csharp
public enum DynamicFilterType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| AboveAverage | `0` | Ortalamanın üzerindeki değerleri gösterir. |
| BelowAverage | `1` | Ortalamanın altındaki değerleri gösterir. |
| LastMonth | `2` | Geçen ayın tarihlerini gösterir. |
| LastQuarter | `3` | Geçen çeyreğin tarihlerini gösterir. |
| LastWeek | `4` | Geçen haftanın tarihlerini gösterir. |
| LastYear | `5` | Geçen yılın tarihlerini gösterir |
| January | `6` | Yıla bakılmaksızın Ocak ayındaki tarihleri gösterir |
| October | `7` | Ekim ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| November | `8` | Kasım ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| December | `9` | Aralık ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| February | `10` | Şubat ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| March | `11` | Mart ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| April | `12` | Nisan ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| May | `13` | Mayıs ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| June | `14` | Haziran ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| July | `15` | Temmuz ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| August | `16` | Ağustos ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| September | `17` | Eylül ayında olan tarihleri, yıl fark etmeksizin gösterir. |
| NextMonth | `18` | Gelecek ayın tarihlerini gösterir. |
| NextQuarter | `19` | Gelecek çeyreğin tarihlerini gösterir. |
| NextWeek | `20` | Gelecek haftanın tarihlerini gösterir. |
| NextYear | `21` | Gelecek yılın tarihlerini gösterir. |
| None | `22` | Hiçbiri. |
| Quarter1 | `23` | 1. çeyrekteki tarihleri, yıl fark etmeksizin gösterir. |
| Quarter2 | `24` | 2. çeyrekteki tarihleri, yıl fark etmeksizin gösterir. |
| Quarter3 | `25` | 3. çeyrekteki tarihleri, yıl fark etmeksizin gösterir. |
| Quarter4 | `26` | 4. çeyrekteki tarihleri, yıl fark etmeksizin gösterir. |
| ThisMonth | `27` | Bu ayın tarihlerini gösterir. |
| ThisQuarter | `28` | Bu çeyreğin tarihlerini gösterir. |
| ThisWeek | `29` | Bu haftanın tarihlerini gösterir. |
| ThisYear | `30` | Bu yılın tarihlerini gösterir. |
| Today | `31` | Bugünün tarihlerini gösterir. |
| Tomorrow | `32` | Yarının tarihlerini gösterir. |
| YearToDate | `33` | Yılın başı ile bugünün tarihleri arasındaki tarihleri, dahil olmak üzere gösterir. |
| Yesterday | `34` | Dünün tarihlerini gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterTypeDemo
    {
        public static void DynamicFilterTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            // Çalışma sayfasına otomatik filtre uygula
            worksheet.AutoFilter.SetRange(0, 0, 5);

            // Sadece Mart ayındaki tarihleri göstermek için dinamik bir filtre uygula
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            // Çalışma kitabını kaydedin
            workbook.Save("DynamicFilterTypeExample.xlsx");
            workbook.Save("DynamicFilterTypeExample.pdf");

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Dynamic filter applied to show only dates in March.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


