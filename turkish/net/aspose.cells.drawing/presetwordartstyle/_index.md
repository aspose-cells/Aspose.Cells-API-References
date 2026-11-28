---
title: "PresetWordArtStyle enum"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.PresetWordArtStyle enum. Önceden ayarlanmış WordArt stillerini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/presetwordartstyle/
---
## PresetWordArtStyle enumeration

Ön ayarlı WordArt stillerini temsil eder.

```csharp
public enum PresetWordArtStyle
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| WordArtStyle1 | `1` | Dolgu - Siyah, Metin 1, Gölge |
| WordArtStyle2 | `2` | Dolgu - Mavi, Vurgu 1, Gölge |
| WordArtStyle3 | `3` | Dolgu - Turuncu, Vurgu 2, Çerçeve - Vurgu 2 |
| WordArtStyle4 | `4` | Dolgu - Beyaz, Çerçeve - Vurgu 1, Gölge |
| WordArtStyle5 | `5` | Dolgu - Altın, Vurgu 4, Yumuşak Köşebent |
| WordArtStyle6 | `6` | Gradyan Dolgu - Gri |
| WordArtStyle7 | `7` | Gradyan Dolgu - Mavi, Vurgu 1, Yansıma |
| WordArtStyle8 | `8` | Gradyan Dolgu - Altın, Vurgu 4, Çerçeve - Vurgu 4 |
| WordArtStyle9 | `9` | Dolgu - Beyaz, Çerçeve - Vurgu 1, Parıltı - Vurgu 1 |
| WordArtStyle10 | `10` | Dolgu - Gri-%50, Vurgu 3, Keskin Köşebent |
| WordArtStyle11 | `11` | Dolgu - Siyah, Metin 1, Çerçeve - Arka Plan 1, Sert Gölge - Arka Plan 1 |
| WordArtStyle12 | `12` | Dolgu - Siyah, Metin 1, Çerçeve - Arka Plan 1, Sert Gölge - Vurgu 1 |
| WordArtStyle13 | `13` | Dolgu - Mavi, Vurgu 1, Çerçeve - Arka Plan 1, Sert Gölge - Vurgu 1 |
| WordArtStyle14 | `14` | Dolgu - Beyaz, Çerçeve - Vurgu 2, Sert Gölge - Vurgu 2 |
| WordArtStyle15 | `15` | Dolgu - Gri-25%, Arka Plan 2, İç Gölge |
| WordArtStyle16 | `16` | Desen Dolgu - Beyaz, Metin 2, Koyu Yukarı Diyagonal, Gölge |
| WordArtStyle17 | `17` | Desen Dolgu - Gri-50%, Vurgu 3, Dar Yatay, İç Gölge |
| WordArtStyle18 | `18` | Dolgu - Mavi, Vurgu 1, %50, Sert Gölge - Vurgu 1 |
| WordArtStyle19 | `19` | Desen Dolgu - Mavi, Vurgu 1, Açık Aşağı Diyagonal, Çerçeve - Vurgu 1 |
| WordArtStyle20 | `20` | Desen Dolgu - Mavi-Gri, Metin 2, Koyu Yukarı Diyagonal, Sert Gölge - Metin 2 |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PresetWordArtStyleDemo
    {
        public static void PresetWordArtStyleExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasının şekil koleksiyonuna erişin
            ShapeCollection shapes = worksheet.Shapes;
            
            // Belirli bir ön ayar stiline sahip bir WordArt şekli ekleyin
            // Parametreler: stil, metin, üstSolSatır, üst, üstSolSütun, sol, yükseklik, genişlik
            Shape wordArt = shapes.AddWordArt(PresetWordArtStyle.WordArtStyle2, "Hello Aspose!", 1, 0, 1, 0, 100, 400);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PresetWordArtStyleExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


