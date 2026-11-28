---
title: "SparklineGroupCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineGroupCollection özelliği. Belirtilen indeksteki SparklineGroup öğesini alır."
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroupcollection/item/
---
## SparklineGroupCollection indexer

Belirtilen indeksteki [`SparklineGroup`](../../sparklinegroup/) öğesini alır.

```csharp
public SparklineGroup this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Örnek veri ekleyin.
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            ws.Cells["A3"].PutValue(7);
            ws.Cells["A4"].PutValue(2);
            ws.Cells["A5"].PutValue(9);

            // Sparklinelar için veri aralığını ve konumu tanımla
            string dataRange = "'" + ws.Name + "'!A1:A5";
            CellArea location = new CellArea();
            location.StartRow = 0;
            location.EndRow = 0;
            location.StartColumn = 1;
            location.EndColumn = 1;

            // Sparkline grubu ekle
            int index = ws.SparklineGroups.Add(SparklineType.Line, dataRange, false, location);
            
            // Item özelliğini kullanarak sparkline grubuna erişin
            SparklineGroup group = ws.SparklineGroups[index];
            
            // Sparkline'ı özelleştirin
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Çalışma kitabını kaydedin
            wb.Save("SparklineGroupCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


