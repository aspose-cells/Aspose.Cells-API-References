---
title: "Range.Merge"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة النطاق. تجمع نطاقًا من الخلايا في خلية واحدة"
type: docs
url: /ar/net/aspose.cells/range/merge/
---
## Range.Merge method

يجمع نطاقًا من الخلايا في خلية واحدة.

```csharp
public void Merge()
```

### ملاحظات

الإشارة إلى الخلية المدمجة عبر عنوان الخلية العليا اليسرى في النطاق.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMergeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق ودمج الخلايا (3 صفوف × 2 أعمدة)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            range.Merge();

            // تعيين القيمة في الخلية المدمجة
            worksheet.Cells[0, 0].Value = "Merged Cells Demo";

            // تنسيق الخلايا المدمجة
            Style style = worksheet.Cells[0, 0].GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.IsBold = true;
            worksheet.Cells[0, 0].SetStyle(style);

            // احفظ المصنف
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


