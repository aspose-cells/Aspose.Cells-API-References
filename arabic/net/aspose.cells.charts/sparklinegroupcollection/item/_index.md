---
title: "SparklineGroupCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroupCollection. تحصل على عنصر SparklineGroup عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroupcollection/item/
---
## SparklineGroupCollection indexer

تحصل على عنصر [`SparklineGroup`](../../sparklinegroup/) عند الفهرس المحدد.

```csharp
public SparklineGroup this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // أضف بيانات تجريبية
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            ws.Cells["A3"].PutValue(7);
            ws.Cells["A4"].PutValue(2);
            ws.Cells["A5"].PutValue(9);

            // حدد نطاق البيانات والموقع لـ sparklines
            string dataRange = "'" + ws.Name + "'!A1:A5";
            CellArea location = new CellArea();
            location.StartRow = 0;
            location.EndRow = 0;
            location.StartColumn = 1;
            location.EndColumn = 1;

            // أضف مجموعة سباركلين
            int index = ws.SparklineGroups.Add(SparklineType.Line, dataRange, false, location);
            
            // الوصول إلى مجموعة المخطط الصغير باستخدام خاصية Item
            SparklineGroup group = ws.SparklineGroups[index];
            
            // تخصيص المخطط الصغير
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // احفظ المصنف
            wb.Save("SparklineGroupCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


