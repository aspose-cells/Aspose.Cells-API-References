---
title: "SparklineGroup.PlotEmptyCellsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineGroup özelliği. Boş hücrelerin nasıl çizileceğini gösterir"
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroup/plotemptycellstype/
---
## SparklineGroup.PlotEmptyCellsType property

Boş hücrelerin nasıl çizileceğini belirtir.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPlotEmptyCellsTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Bazı boş hücreler içeren veri ekle
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(null); // Empty cell
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Sparkline için CellArea'yı tanımla
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Bir sparkline grubu ekle
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Boş hücrelerin nasıl çizileceğini ayarla
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;

            // Sparkline'ı gruba ekle
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Çalışma kitabını kaydedin
            workbook.Save("SparklineEmptyCellsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


