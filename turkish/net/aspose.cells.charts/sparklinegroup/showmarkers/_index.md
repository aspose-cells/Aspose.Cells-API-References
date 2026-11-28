---
title: "SparklineGroup.ShowMarkers"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineGroup özelliği. Sparkline grubundaki her satır sparkline'ındaki her noktayı vurgulayıp vurgulamama durumunu gösterir."
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroup/showmarkers/
---
## SparklineGroup.ShowMarkers property

Sparkline grubundaki her satır sparkline'ındaki her noktayı vurgulayıp vurgulanmayacağını gösterir.

```csharp
public bool ShowMarkers { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowMarkersDemo
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

            // Sparkline ekle
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Sparkline görünümünü yapılandır
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            group.ShowMarkers = true;
            
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            // Çalışma kitabını kaydedin
            workbook.Save("SparklineWithMarkers.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


