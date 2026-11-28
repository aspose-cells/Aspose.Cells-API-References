---
title: "Enum PlacementType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.PlacementType enum. Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/placementtype/
---
## PlacementType enumeration

Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder.

```csharp
public enum PlacementType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| FreeFloating | `0` | Hücrelerle birlikte hareket etmeyin veya boyutlandırmayın. |
| Move | `1` | Hücrelerle birlikte hareket edin ancak boyutlandırmayın. |
| MoveAndSize | `2` | Hücrelerle birlikte hareket edin ve boyutlandırın. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class PlacementTypeDemo
    {
        public static void PlacementTypeExample()
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

            // Grafiğin yerleştirme tipini ayarlayın
            chart.Placement = PlacementType.MoveAndSize;

            // Yerleştirme tipini çıktı olarak verin
            Console.WriteLine("Chart Placement Type: " + chart.Placement);

            // Çalışma kitabını kaydedin
            workbook.Save("PlacementTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


