---
title: "Enum PresetMaterialType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.PresetMaterialType enum. Bir şeklin yüzey görünümünü tanımlar"
type: docs
url: /tr/net/aspose.cells.drawing/presetmaterialtype/
---
## PresetMaterialType enumeration

Bir şeklin yüzey görünümünü tanımlar.

```csharp
public enum PresetMaterialType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Clear | `0` | Temiz |
| DarkEdge | `1` | Koyu kenar |
| Flat | `2` | Düz |
| LegacyMatte | `3` | Eski mat |
| LegacyMetal | `4` | Eski metal |
| LegacyPlastic | `5` | Eski plastik |
| LegacyWireframe | `6` | Eski tel kafes |
| Matte | `7` | Mat |
| Metal | `8` | Metal |
| Plastic | `9` | Plastik |
| Powder | `10` | Toz |
| SoftEdge | `11` | Yumuşak kenar |
| SoftMetal | `12` | Yumuşak metal |
| TranslucentPowder | `13` | Şeffaf toz |
| WarmMatte | `14` | Sıcak mat |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class PresetMaterialTypeDemo
    {
        public static void PresetMaterialTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            // Grafikteki ilk seriye eriş
            Series series = chart.NSeries[0];

            // Serinin 3B formatına eriş
            Format3D format3D = series.ShapeProperties.Format3D;

            // Yüzey malzeme tipini ayarla
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;

            // Diğer 3B özellikleri ayarla
            format3D.LightingAngle = 45;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;

            // Çalışma kitabını kaydedin
            workbook.Save("PresetMaterialTypeExample.xlsx");

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Chart with 3D format and PresetMaterialType applied has been created.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


