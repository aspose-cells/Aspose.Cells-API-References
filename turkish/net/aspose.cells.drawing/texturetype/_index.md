---
title: "Enum TextureType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.TextureType enum. Önceden tanımlı doku tipini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing/texturetype/
---
## TextureType enumeration

Önceden ayarlanmış doku türünü temsil eder.

```csharp
public enum TextureType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| BlueTissuePaper | `0` | Mavi Kağıt Havlu doku tipini temsil eder. |
| Bouquet | `1` | Buket doku tipini temsil eder. |
| BrownMarble | `2` | Kahverengi Mermer doku tipini temsil eder. |
| Canvas | `3` | Kanvas doku tipini temsil eder. |
| Cork | `4` | Mantar doku tipini temsil eder. |
| Denim | `5` | Denim doku tipini temsil eder. |
| FishFossil | `6` | Balık Fosili doku tipini temsil eder. |
| Granite | `7` | Granit doku tipini temsil eder. |
| GreenMarble | `8` | Yeşil Mermer doku tipini temsil eder. |
| MediumWood | `9` | Orta Ahşap doku tipini temsil eder. |
| Newsprint | `10` | Gazete Kağıdı doku tipini temsil eder. |
| Oak | `11` | Meşe doku tipini temsil eder. |
| PaperBag | `12` | Kağıt Torba doku tipini temsil eder. |
| Papyrus | `13` | Papirüs doku tipini temsil eder. |
| Parchment | `14` | Parşömen doku tipini temsil eder. |
| PinkTissuePaper | `15` | Pembe Kağıt Havlu doku tipini temsil eder. |
| PurpleMesh | `16` | Mor Ağ doku tipini temsil eder. |
| RecycledPaper | `17` | Geri Dönüştürülmüş Kağıt doku tipini temsil eder. |
| Sand | `18` | Kum doku tipini temsil eder. |
| Stationery | `19` | Stationery doku tipini temsil eder. |
| Walnut | `20` | Walnut Droplets doku tipini temsil eder. |
| WaterDroplets | `21` | Water Droplets doku tipini temsil eder. |
| WhiteMarble | `22` | White Marble doku tipini temsil eder. |
| WovenMat | `23` | Woven Mat doku tipini temsil eder. |
| Unknown | `24` | Bilinmeyen doku tipini temsil eder. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextureTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seriye erişin ve bir nokta için dokuyu ayarlayın
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Stationery;

            // Çalışma kitabını kaydedin
            workbook.Save("TextureTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


