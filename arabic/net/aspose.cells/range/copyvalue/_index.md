---
title: "Range.CopyValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. ينسخ قيمة الخلية من نطاق مصدر"
type: docs
url: /ar/net/aspose.cells/range/copyvalue/
---
## Range.CopyValue method

ينسخ قيمة الخلية من نطاق مصدر.

```csharp
public void CopyValue(Range range)
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
    public class RangeMethodCopyValueWithRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل والحصول على ورقة العمل الأولى
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "SourceSheet";
            
            // إضافة ورقة عمل أخرى للوجهة
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "DestinationSheet";
            
            // إنشاء بيانات عينة في النطاق المصدر
            Cells cellsSrc = sheetSrc.Cells;
            cellsSrc["A1"].PutValue("Source Data");
            cellsSrc["A2"].PutValue(10);
            cellsSrc["B2"].PutValue(20);
            cellsSrc["A3"].PutValue(30);
            cellsSrc["B3"].PutValue(40);
            
            // إنشاء نطاقات للمصدر والوجهة
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A2:B3");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("D2:E3");
            
            // نسخ القيم من النطاق المصدر إلى النطاق الوجهة
            rangeDest.CopyValue(rangeSrc);
            
            // احفظ المصنف
            workbook.Save("RangeCopyValueDemo.xlsx");
            
            Console.WriteLine("Values copied successfully from source range to destination range.");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


