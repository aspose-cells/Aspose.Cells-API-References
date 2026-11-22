---
title: "ChartDataTable.HasBorderHorizontal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartDataTable. True إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية"
type: docs
url: /ar/net/aspose.cells.charts/chartdatatable/hasborderhorizontal/
---
## ChartDataTable.HasBorderHorizontal property

صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية

```csharp
[Obsolete("Use ChartDataTable.HasHorizontalBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderHorizontal { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ChartDataTable.HasHorizontalBorder. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يونيو 2024. شركة Aspose تعتذر عن أي إزعاج قد تكون قد واجهته.

### أمثلة

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

### انظر أيضًا

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


