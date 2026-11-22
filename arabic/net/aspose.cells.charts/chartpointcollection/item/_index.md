---
title: "ChartPointCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPointCollection. يحصل على عنصر ChartPoint عند الفهرس المحدد في السلسلة"
type: docs
url: /ar/net/aspose.cells.charts/chartpointcollection/item/
---
## ChartPointCollection indexer

يحصل على عنصر [`ChartPoint`](../../chartpoint/) عند الفهرس المحدد في السلسلة.

```csharp
public ChartPoint this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | فهرس نقطة المخطط في السلسلة. |

### قيمة الإرجاع

كائن ChartPoint.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى نقطة مخطط محددة باستخدام خاصية Item
            ChartPoint point = chart.NSeries[0].Points[1];
            
            // تعديل نمط تعبئة النقطة
            point.Area.FillFormat.Pattern = FillPattern.LightHorizontal;

            // احفظ المصنف
            workbook.Save("ChartPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../../chartpoint/)
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


