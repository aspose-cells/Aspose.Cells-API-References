---
title: "SparklineGroup.ShowNegativePoints"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineGroup özelliği. Sparkline grubundaki negatif değerleri farklı bir renk veya işaretçi ile vurgulayıp vurgulamayacağını gösterir."
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroup/shownegativepoints/
---
## SparklineGroup.ShowNegativePoints property

Sparkline grubundaki negatif değerleri farklı bir renk veya işaretçi ile vurgulayıp vurgulanmayacağını gösterir.

```csharp
public bool ShowNegativePoints { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowNegativePointsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // ShowNegativePoints özelliğini göstermek için negatif değerli veri ekle.
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(-2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(-3);

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

            // Sparkline grup özelliklerini yapılandır
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            // Çalışma kitabını kaydedin
            workbook.Save("SparklineNegativePointsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


