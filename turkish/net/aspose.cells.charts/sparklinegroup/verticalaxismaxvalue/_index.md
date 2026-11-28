---
title: "SparklineGroup.VerticalAxisMaxValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineGroup özelliği. Dikey eksen için özel maksimum değeri alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroup/verticalaxismaxvalue/
---
## SparklineGroup.VerticalAxisMaxValue property

Dikey eksen için özel maksimum değeri alır ve ayarlar.

```csharp
public double VerticalAxisMaxValue { get; set; }
```

### Açıklamalar

Bu özellik ayarlanırsa, [`VerticalAxisMaxValueType`](../verticalaxismaxvaluetype/) Custom olacaktır.

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMaxValueDemo
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

            // Dikey eksen maksimum değerini ayarla
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMaxValue = 10.0;

            // Çalışma kitabını kaydedin
            workbook.Save("SparklineVerticalAxisMaxValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


