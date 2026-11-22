---
title: "Range.CopyData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. نسخ بيانات الخلية بما في ذلك الصيغ من نطاق المصدر"
type: docs
url: /ar/net/aspose.cells/range/copydata/
---
## Range.CopyData method

ينسخ بيانات الخلية (بما في ذلك الصيغ) من نطاق مصدر.

```csharp
public void CopyData(Range range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| range | Range | كائن المصدر [`Range`](../). |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyDataWithRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على ورقة العمل الأولى وأضف بعض البيانات
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            sheetSrc.Cells["A1"].PutValue("Source Data");
            sheetSrc.Cells["B1"].PutValue(100);
            sheetSrc.Cells["A2"].PutValue("More Data");
            sheetSrc.Cells["B2"].PutValue(200);

            // أضف ورقة عمل وجهة
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";

            // إنشاء نطاقات المصدر والوجهة
            Aspose.Cells.Range rangeSrc = sheetSrc.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("C3:D4");

            // نسخ البيانات من النطاق المصدر إلى النطاق الوجهة
            rangeDest.CopyData(rangeSrc);

            // احفظ المصنف
            workbook.Save("RangeCopyDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


