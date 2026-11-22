---
title: "ChartDataTable.HasBorderOutline"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartDataTable. صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خارجية"
type: docs
url: /ar/net/aspose.cells.charts/chartdatatable/hasborderoutline/
---
## ChartDataTable.HasBorderOutline property

صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خارجية

```csharp
[Obsolete("Use ChartDataTable.HasOutlineBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderOutline { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت مهجورة الآن. بدلاً من ذلك، يرجى استخدام خاصية ChartDataTable.HasOutlineBorder. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasBorderOutlineDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // تمكين وتكوين جدول البيانات
            chart.ShowDataTable = true;
            ChartDataTable chartTable = chart.ChartDataTable;
            
            // عرض خاصية HasBorderOutline
            chartTable.HasBorderOutline = true;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.Font.Color = Color.Blue;

            workbook.Save("ChartDataTableWithBorderOutline.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


