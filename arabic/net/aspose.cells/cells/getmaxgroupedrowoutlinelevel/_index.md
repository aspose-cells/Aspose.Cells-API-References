---
title: "Cells.GetMaxGroupedRowOutlineLevel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على أقصى مستوى مخطط للصفوف المجمعة بصفرية"
type: docs
url: /ar/net/aspose.cells/cells/getmaxgroupedrowoutlinelevel/
---
## Cells.GetMaxGroupedRowOutlineLevel method

يحصل على الحد الأقصى لمستوى مخطط الصف المجمّع (بدءًا من الصفر).

```csharp
public int GetMaxGroupedRowOutlineLevel()
```

### قيمة الإرجاع

أقصى مستوى مخطط للصف المجمّع (صفرية)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedRowOutlineLevelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // قم بتجميع بعض الصفوف لتوضيح مستويات المخطط
            cells.GroupRows(0, 2, false);
            cells.GroupRows(4, 6, false);
            
            // إضافة تجميع متداخل
            cells.GroupRows(4, 5, true);

            // احصل على أقصى مستوى مخطط للصف المجمّع
            int maxOutlineLevel = cells.GetMaxGroupedRowOutlineLevel();

            // اعرض النتيجة
            Console.WriteLine("Maximum grouped row outline level: " + maxOutlineLevel);

            // عرض مستوى المخطط لكل صف
            for (int row = 0; row <= 6; row++)
            {
                Console.WriteLine($"Row {row} outline level: {cells.GetGroupedRowOutlineLevel(row)}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


