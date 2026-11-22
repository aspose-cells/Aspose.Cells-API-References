---
title: "Range.MoveTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تحرك النطاق الحالي إلى النطاق الوجهة"
type: docs
url: /ar/net/aspose.cells/range/moveto/
---
## Range.MoveTo method

انقل النطاق الحالي إلى النطاق الوجهة.

```csharp
public void MoveTo(int destRow, int destColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destRow | Int32 | صف البداية للنطاق الوجهة. |
| destColumn | Int32 | عمود البداية للنطاق الوجهة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق مثال (A1:B2)
            Aspose.Cells.Range originalRange = worksheet.Cells.CreateRange("A1", "B2");
            
            // ضع بعض البيانات في النطاق للتوضيح
            originalRange[0, 0].PutValue("A1");
            originalRange[0, 1].PutValue("B1");
            originalRange[1, 0].PutValue("A2");
            originalRange[1, 1].PutValue("B2");
            
            // حرك النطاق للأسفل بمقدار صف واحد (إلى A2:B3)
            originalRange.MoveTo(originalRange.FirstRow + 1, originalRange.FirstColumn);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


