---
title: "SparklineCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineCollection yöntemi. Bir sparkline ekle"
type: docs
url: /tr/net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

Bir sparkline ekle.

```csharp
public int Add(string dataRange, int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataRange | String | Sparkline'in yeni veri aralığını belirtir. |
| satır | Int32 | Konumun satır indeksi. |
| sütun | Int32 | Konumun sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            for (int i = 0; i < 12; i++)
            {
                worksheet.Cells[4, 3 + i].PutValue(i + 1);
            }

            // Bir sparkline grubu oluştur
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Veri aralığı ve konum ile sparkline ekle
            int sparklineIndex = group.Sparklines.Add("D5:O5", 4, 15);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


