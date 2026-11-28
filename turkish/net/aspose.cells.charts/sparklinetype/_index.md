---
title: "Enum SparklineType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.SparklineType enum. Sparkline türlerini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/sparklinetype/
---
## SparklineType enumeration

Sparkline türlerini temsil eder.

```csharp
public enum SparklineType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Line | `0` | Çizgi sparkline. |
| Column | `1` | Sütun kıvırcık grafiği. |
| Stacked | `2` | Bir Kazanç/Kayıp kıvırcık grafiğini temsil eder. |
| WinLoss | `2` | Bir Kazanç/Kayıp kıvırcık grafiğini temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineTypeDemo
    {
        public static void SparklineTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Sparkline için CellArea'yı tanımla
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Çalışma sayfasına bir sparkline grubu ekle
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];

            // Gruba sparkline'lar ekle
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Kıvırcık grafik grubunu özelleştir
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;

            // Yüksek noktaları yeşile, düşük noktaları kırmızıya renklendirin
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;

            // Çizgi kalınlığını ayarla
            group.LineWeight = 1.0;

            // Çalışma kitabını kaydedin
            workbook.Save("SparklineTypeExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


