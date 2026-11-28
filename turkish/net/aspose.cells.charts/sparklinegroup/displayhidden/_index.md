---
title: "SparklineGroup.DisplayHidden"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineGroup özelliği. Gizli satır ve sütunlardaki verilerin gösterilip gösterilmeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroup/displayhidden/
---
## SparklineGroup.DisplayHidden property

Gizli satır ve sütunlardaki verilerin gösterilip gösterilmeyeceğini belirtir.

```csharp
public bool DisplayHidden { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyDisplayHiddenDemo
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

            // Sparkline konumunu tanımla
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Sparkline grubu ekle
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Sparkline'ı gruba ekle
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Sparkline görünümünü yapılandır
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Blue;
            group.SeriesColor = seriesColor;

            // DisplayHidden özelliğini göster
            group.DisplayHidden = true; // Show sparklines for hidden data

            // Çalışma kitabını kaydedin
            workbook.Save("SparklineDisplayHiddenDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


