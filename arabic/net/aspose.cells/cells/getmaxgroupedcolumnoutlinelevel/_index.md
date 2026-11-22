---
title: "Cells.GetMaxGroupedColumnOutlineLevel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على أقصى مستوى مخطط للعمود المجموع بدءًا من الصفر"
type: docs
url: /ar/net/aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/
---
## Cells.GetMaxGroupedColumnOutlineLevel method

يحصل على الحد الأقصى لمستوى مخطط العمود المجمّع (بدءًا من الصفر).

```csharp
public int GetMaxGroupedColumnOutlineLevel()
```

### قيمة الإرجاع

أقصى مستوى مخطط للعمود المجموع (بدءًا من الصفر)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedColumnOutlineLevelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // قم بتجميع بعض الأعمدة لتوضيح مستويات المخطط
            cells.GroupColumns(0, 2, false);
            cells.GroupColumns(3, 5, false);
            
            // احصل على أقصى مستوى مخطط للعمود المجموع
            int maxOutlineLevel = cells.GetMaxGroupedColumnOutlineLevel();
            
            Console.WriteLine("Maximum grouped column outline level: " + maxOutlineLevel);
            
            // عرض مستوى المخطط لكل عمود
            for (int col = 0; col < 6; col++)
            {
                int outlineLevel = cells.GetGroupedColumnOutlineLevel(col);
                Console.WriteLine($"Column {col} outline level: {outlineLevel}");
            }
            
            // احفظ المصنف
            workbook.Save("GroupedColumnsOutlineLevel.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


