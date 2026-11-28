---
title: "Sparkline.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Sparkline özelliği. Sparkline'ın satır indeksini alır"
type: docs
url: /tr/net/aspose.cells.charts/sparkline/row/
---
## Sparkline.Row property

Sparkline'ın satır indeksini alır.

```csharp
public int Row { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Sparkline grubu oluştur
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Satır 0, sütun 4'te bir sparkline ekle
            int sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Satır konumunu göster (yalnızca okunabilir özellik)
            Console.WriteLine("Sparkline row position: " + sparkline.Row);

            // Konumu değiştirmek için sparkline'ı kaldırıp yeniden oluşturmalıyız
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 2, 4); // New position at row 2
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New sparkline row position: " + sparkline.Row);

            // Çalışma kitabını kaydet
            workbook.Save("SparklineRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


