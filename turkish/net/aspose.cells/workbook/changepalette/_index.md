---
title: "Workbook.ChangePalette"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Belirtilen indeksteki elektronik tablo için renk paletini değiştirir"
type: docs
url: /tr/net/aspose.cells/workbook/changepalette/
---
## Workbook.ChangePalette method

Belirtilen indeksteki elektronik tablo için paleti değiştirir.

```csharp
public void ChangePalette(Color color, int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | Color | Renk yapısı. |
| indeks | Int32 | Palet indeksi, 0 - 55. |

### Açıklamalar

Palet 56 girdi içerir, her biri bir RGB değeriyle temsil edilir.

Palet içinde olmayan bir renk ayarlarsanız, etkili olmayacaktır.

Bu yüzden özel bir renk ayarlamak istiyorsanız, önce paleti değiştirin.

Aşağıdaki standart renk paletidir.

| **Color** | **Red** | **Yeşil** | **Mavi** |
| --- | --- | --- | --- |
| Siyah | 0 | 0 | 0 |
| Beyaz | 255 | 255 | 255 |
| Kırmızı | 255 | 0 | 0 |
| Limon | 0 | 255 | 0 |
| Mavi | 0 | 0 | 255 |
| Sarı | 255 | 255 | 0 |
| Macenta | 255 | 0 | 255 |
| Camgöbeği | 0 | 255 | 255 |
| Kestane | 128 | 0 | 0 |
| Yeşil | 0 | 128 | 0 |
| Lacivert | 0 | 0 | 128 |
| Zeytin | 128 | 128 | 0 |
| Mor | 128 | 0 | 128 |
| Turkuaz | 0 | 128 | 128 |
| Gümüş | 192 | 192 | 192 |
| Gri | 128 | 128 | 128 |
| Renk17 | 153 | 153 | 255 |
| Renk18 | 153 | 51 | 102 |
| Renk19 | 255 | 255 | 204 |
| Renk20 | 204 | 255 | 255 |
| Renk21 | 102 | 0 | 102 |
| Renk22 | 255 | 128 | 128 |
| Renk23 | 0 | 102 | 204 |
| Renk24 | 204 | 204 | 255 |
| Renk25 | 0 | 0 | 128 |
| Renk26 | 255 | 0 | 255 |
| Renk27 | 255 | 255 | 0 |
| Renk28 | 0 | 255 | 255 |
| Renk29 | 128 | 0 | 128 |
| Renk30 | 128 | 0 | 0 |
| Renk31 | 0 | 128 | 128 |
| Renk32 | 0 | 0 | 255 |
| Renk33 | 0 | 204 | 255 |
| Renk34 | 204 | 255 | 255 |
| Renk35 | 204 | 255 | 204 |
| Renk36 | 255 | 255 | 153 |
| Renk37 | 153 | 204 | 255 |
| Renk38 | 255 | 153 | 204 |
| Renk39 | 204 | 153 | 255 |
| Renk40 | 255 | 204 | 153 |
| Renk41 | 51 | 102 | 255 |
| Renk42 | 51 | 204 | 204 |
| Renk43 | 153 | 204 | 0 |
| Color44 | 255 | 204 | 0 |
| Color45 | 255 | 153 | 0 |
| Color46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodChangePaletteWithColorInt32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı örneği oluştur
            Workbook workbook = new Workbook();
            
            // 55. indeksteki palet rengini değiştir
            Color newColor = Color.FromArgb(255, 250, 223);
            workbook.ChangePalette(newColor, 55);

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Değiştirilmiş palet rengiyle bir stil oluştur
            Style style = workbook.CreateStyle();
            style.ForegroundColor = newColor;
            style.Pattern = BackgroundType.Solid;

            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Palette Color Demo");
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("ChangePaletteDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


