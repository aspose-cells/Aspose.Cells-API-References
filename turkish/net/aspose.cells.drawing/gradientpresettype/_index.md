---
title: "Enum GradientPresetType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.GradientPresetType enum. Degrade ön ayar renk tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/gradientpresettype/
---
## GradientPresetType enumeration

Degrade ön ayar renk tipini temsil eder.

```csharp
public enum GradientPresetType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Brass | `0` | Pirinç ön ayar rengi |
| CalmWater | `1` | Sakin Su ön ayar rengi |
| Chrome | `2` | Krom ön ayar rengi |
| ChromeII | `3` | Krom II ön ayar rengi |
| Daybreak | `4` | Şafak ön ayar rengi |
| Desert | `5` | Çöl ön ayar rengi |
| EarlySunset | `6` | Erken Gün Batımı ön ayar rengi |
| Fire | `7` | Ateş ön ayar rengi |
| Fog | `8` | Sis ön ayar rengi |
| Gold | `9` | Altın ön ayar rengi |
| GoldII | `10` | Altın II ön ayar rengi |
| Horizon | `11` | Ufuk ön ayar rengi |
| LateSunset | `12` | Geç Gün Batımı ön ayar rengi |
| Mahogany | `13` | Mahoni ön ayar rengi |
| Moss | `14` | Yosun ön ayar rengi |
| Nightfall | `15` | Alacakaranlık ön ayar rengi |
| Ocean | `16` | Okyanus ön ayar rengi |
| Parchment | `17` | Parşömen ön ayar rengi |
| Peacock | `18` | Tavus kuşu ön ayar rengi |
| Rainbow | `19` | Gökkuşağı ön ayar rengi |
| RainbowII | `20` | Gökkuşağı II ön ayar rengi |
| Sapphire | `21` | Safir ön ayar rengi |
| Silver | `22` | Gümüş ön ayar rengi |
| Wheat | `23` | Buğday ön ayar rengi |
| Unknown | `24` | Bilinmeyen ön ayar rengi. Yalnızca şablon çalışma kitabındaki ön ayar rengi (bilinen hiçbir ön ayar rengiyle aynı olmayan) için. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientPresetTypeDemo
    {
        public static void GradientPresetTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            // Grafiğin kategori eksenine erişin
            Axis categoryAxis = chart.CategoryAxis;

            // Kategori eksen alanının doldurma biçimine erişin
            FillFormat fillFormat = categoryAxis.Area.FillFormat;

            // Doldurma biçimi için bir degrade ön ayar rengi ayarlayın
            fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);

            // Degrade ön ayar renk tipini çıktı olarak verin
            Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);

            // Çalışma kitabını kaydedin
            workbook.Save("GradientPresetTypeExample.xlsx");
            workbook.Save("GradientPresetTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


