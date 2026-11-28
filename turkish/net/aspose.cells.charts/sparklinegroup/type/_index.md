---
title: "SparklineGroup.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineGroup özelliği. Sparkline grubunun sparkline tipini gösterir"
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroup/type/
---
## SparklineGroup.Type property

Sparkline grubunun sparkline tipini gösterir.

```csharp
public SparklineType Type { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyTypeDemo
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

            // Column tipiyle sparkline grubu oluştur
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Column, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Sparkline tipini Line olarak değiştir
            group.Type = SparklineType.Line;

            // Sparkline'ı gruba ekle
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Çalışma kitabını kaydedin
            workbook.Save("SparklineTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


