---
title: "Enum FillPattern"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.FillPattern enum. Şekil dolgu deseni türlerini sıralar"
type: docs
url: /tr/net/aspose.cells.drawing/fillpattern/
---
## FillPattern enumeration

Şekil dolgu desen türlerini sıralar.

```csharp
public enum FillPattern
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Arka plan yoktur. |
| Solid | `1` | Düz desenini temsil eder. |
| Gray5 | `2` | %5 gri desenini temsil eder. |
| Gray10 | `3` | %10 gri desenini temsil eder. |
| Gray20 | `4` | %20 gri desenini temsil eder. |
| Gray30 | `5` | %30 gri desenini temsil eder. |
| Gray40 | `6` | %40 gri desenini temsil eder. |
| Gray50 | `7` | %50 gri desenini temsil eder. |
| Gray60 | `8` | %60 gri desenini temsil eder. |
| Gray70 | `9` | %70 gri desenini temsil eder. |
| Gray75 | `10` | %75 gri desenini temsil eder. |
| Gray80 | `11` | 80% gri deseni temsil eder. |
| Gray90 | `12` | 90% gri deseni temsil eder. |
| Gray25 | `13` | %25 gri desenini temsil eder. |
| LightDownwardDiagonal | `14` | Açık aşağı doğru diyagonal deseni temsil eder. |
| LightUpwardDiagonal | `15` | Açık yukarı doğru diyagonal deseni temsil eder. |
| DarkDownwardDiagonal | `16` | Koyu aşağı doğru diyagonal deseni temsil eder. |
| DarkUpwardDiagonal | `17` | Koyu yukarı doğru diyagonal deseni temsil eder. |
| WideDownwardDiagonal | `18` | Geniş aşağı doğru diyagonal deseni temsil eder. |
| WideUpwardDiagonal | `19` | Geniş yukarı doğru diyagonal deseni temsil eder. |
| LightVertical | `20` | Açık dikey deseni temsil eder. |
| LightHorizontal | `21` | Açık yatay deseni temsil eder. |
| NarrowVertical | `22` | Dar dikey deseni temsil eder. |
| NarrowHorizontal | `23` | Dar yatay deseni temsil eder. |
| DarkVertical | `24` | Koyu dikey deseni temsil eder. |
| DarkHorizontal | `25` | Koyu yatay deseni temsil eder. |
| DashedDownwardDiagonal | `26` | Kesikli aşağı doğru diyagonal deseni temsil eder. |
| DashedUpwardDiagonal | `27` | Kesikli yukarı doğru diyagonal deseni temsil eder. |
| DashedVertical | `28` | Kesikli dikey deseni temsil eder. |
| DashedHorizontal | `29` | Kesikli yatay deseni temsil eder. |
| SmallConfetti | `30` | Küçük konfeti deseni temsil eder. |
| LargeConfetti | `31` | Büyük konfeti deseni temsil eder. |
| ZigZag | `32` | Zikzak deseni temsil eder. |
| Wave | `33` | Dalga deseni temsil eder. |
| DiagonalBrick | `34` | Diyagonal tuğla deseni temsil eder. |
| HorizontalBrick | `35` | Yatay tuğla deseni temsil eder. |
| Weave | `36` | Dokuma deseni temsil eder. |
| Plaid | `37` | Kareli deseni temsil eder. |
| Divot | `38` | Çökük deseni temsil eder. |
| DottedGrid | `39` | Noktalı ızgara desenini temsil eder. |
| DottedDiamond | `40` | Noktalı elmas desenini temsil eder. |
| Shingle | `41` | Shingle desenini temsil eder. |
| Trellis | `42` | Trellis desenini temsil eder. |
| Sphere | `43` | Küre desenini temsil eder. |
| SmallGrid | `44` | Küçük ızgara desenini temsil eder. |
| LargeGrid | `45` | Büyük ızgara desenini temsil eder. |
| SmallCheckerBoard | `46` | Küçük dama tahtası desenini temsil eder. |
| LargeCheckerBoard | `47` | Büyük dama tahtası desenini temsil eder. |
| OutlinedDiamond | `48` | Çerçeveli elmas desenini temsil eder. |
| SolidDiamond | `49` | Dolgun elmas desenini temsil eder. |
| Unknown | `50` | Bilinmeyen deseni temsil eder. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillPatternDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seri için doldurma desenini ayarla
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Plaid;

            // Çalışma kitabını kaydedin
            workbook.Save("FillPatternDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


