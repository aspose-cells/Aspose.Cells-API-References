---
title: "SparklineCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SparklineCollection. إضافة مخطط صغير"
type: docs
url: /ar/net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

أضف sparkline.

```csharp
public int Add(string dataRange, int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataRange | String | يحدد النطاق الجديد للبيانات للمخطط الصغير. |
| صف | Int32 | فهرس الصف للموقع. |
| عمود | Int32 | فهرس العمود للموقع. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            for (int i = 0; i < 12; i++)
            {
                worksheet.Cells[4, 3 + i].PutValue(i + 1);
            }

            // إنشاء مجموعة مخططات صغيرة
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // إضافة مخطط صغير بنطاق البيانات والموقع
            int sparklineIndex = group.Sparklines.Add("D5:O5", 4, 15);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


