---
title: "Enum LightRigType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.LightRigType enum. Bir şekle uygulanabilecek önceden ayarlanmış bir ışık yönünü temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing/lightrigtype/
---
## LightRigType enumeration

Şekle uygulanabilen ön ayarlı sağ ışık yönünü temsil eder

```csharp
public enum LightRigType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Balanced | `0` | Dengeli |
| BrightRoom | `1` | Aydınlık oda |
| Chilly | `2` | Serin |
| Contrasting | `3` | Zıt |
| Flat | `4` | Düz |
| Flood | `5` | Sel |
| Freezing | `6` | Dondurucu |
| Glow | `7` | Parıltı |
| Harsh | `8` | Sert |
| LegacyFlat1 | `9` | LegacyFlat1 |
| LegacyFlat2 | `10` | LegacyFlat2 |
| LegacyFlat3 | `11` | LegacyFlat3 |
| LegacyFlat4 | `12` | LegacyFlat4 |
| LegacyHarsh1 | `13` | LegacyHarsh1 |
| LegacyHarsh2 | `14` | LegacyHarsh2 |
| LegacyHarsh3 | `15` | LegacyHarsh3 |
| LegacyHarsh4 | `16` | LegacyHarsh4 |
| LegacyNormal1 | `17` | LegacyNormal1 |
| LegacyNormal2 | `18` | LegacyNormal2 |
| LegacyNormal3 | `19` | LegacyNormal3 |
| LegacyNormal4 | `20` | LegacyNormal4 |
| Morning | `21` | Sabah |
| Soft | `22` | Yumuşak |
| Sunrise | `23` | Gün doğumu |
| Sunset | `24` | Gün batımı |
| ThreePoint | `25` | Üç nokta |
| TwoPoint | `26` | İki nokta |
| None | `27` | No light rig'i yok. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LightRigTypeDemo
    {
        public static void LightRigTypeExample()
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

            // Grafikteki ilk seriye eriş
            Series series = chart.NSeries[0];

            // Serinin şekil özelliklerine erişin
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Serinin 3B biçim verisine sahip olup olmadığını kontrol edin
            if (shapeProperties.HasFormat3D())
            {
                // 3B format özelliklerine erişin
                Format3D format3D = shapeProperties.Format3D;

                // Yüzey aydınlatma tipini Dengeli olarak ayarlayın
                format3D.SurfaceLightingType = LightRigType.Balanced;

                // Aydınlatma açısını ayarlayın
                format3D.LightingAngle = 45.0;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("LightRigTypeExample.xlsx");
            workbook.Save("LightRigTypeExample.pdf");
            // Sonuçları çıktı olarak ver.
            Console.WriteLine("LightRigType example applied and workbook saved as 'LightRigTypeExample.xlsx'.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


