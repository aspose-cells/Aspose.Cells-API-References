---
title: "Cells.MergedCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل على مجموعة الخلايا المدمجة"
type: docs
url: /ar/net/aspose.cells/cells/mergedcells/
---
## Cells.MergedCells property

يحصل على مجموعة الخلايا المدمجة.

```csharp
[Obsolete("Use Cells.GetMergedAreas() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList MergedCells { get; }
```

### ملاحظات

في هذه المجموعة، كل عنصر هو بنية [`CellArea`](../../cellarea/) تمثل مساحة من الخلايا المدمجة.

ملاحظة: هذه الطريقة أصبحت الآن قديمة. بدلاً من ذلك، يرجى استخدام طريقة Cells.GetMergedAreas(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2023. تُعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsPropertyMergedCellsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // دمج الخلايا في نطاقين مختلفين
            cells.Merge(0, 0, 2, 2); // Merges A1:B2
            cells.Merge(2, 2, 2, 2); // Merges C3:D4

            // الوصول إلى خاصية MergedCells (للقراءة فقط)
            ArrayList mergedRanges = cells.MergedCells;

            // عرض عدد الخلايا المدمجة الأولي والنطاقات
            Console.WriteLine($"Initial merged cells count: {mergedRanges.Count}");
            foreach (CellArea area in mergedRanges)
            {
                Console.WriteLine($"Merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // فك دمج النطاق المدمج الأول
            cells.UnMerge(0, 0, 2, 2);

            // عرض عدد الخلايا المدمجة المحدث والنطاقات
            Console.WriteLine($"\nAfter unmerging A1:B2 - Merged cells count: {cells.MergedCells.Count}");
            foreach (CellArea area in cells.MergedCells)
            {
                Console.WriteLine($"Remaining merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // حفظ النتيجة
            workbook.Save("PropertyMergedCellsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


