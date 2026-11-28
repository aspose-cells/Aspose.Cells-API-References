---
title: "ChartDataTable.HasBorderHorizontal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartDataTable özelliği. Grafik veri tablosunda yatay hücre kenarlıkları varsa True döner."
type: docs
url: /tr/net/aspose.cells.charts/chartdatatable/hasborderhorizontal/
---
## ChartDataTable.HasBorderHorizontal property

Grafik veri tablosunun yatay hücre kenarları varsa doğru

```csharp
[Obsolete("Use ChartDataTable.HasHorizontalBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderHorizontal { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine lütfen ChartDataTable.HasHorizontalBorder özelliğini kullanın. Bu özellik, Haziran 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasBorderHorizontalDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.ShowDataTable = true;

            ChartDataTable chartTable = chart.ChartDataTable;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = false;
            chartTable.HasBorderOutline = false;

            workbook.Save("ChartDataTable_HasBorderHorizontal.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


