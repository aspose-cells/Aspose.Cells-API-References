---
title: "Cells.Rows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل على مجموعة كائنات Row التي تمثل الصفوف الفردية في ورقة العمل هذه"
type: docs
url: /ar/net/aspose.cells/cells/rows/
---
## Cells.Rows property

يحصل على مجموعة كائنات [`Row`](../../row/) التي تمثل الصفوف الفردية في ورقة العمل هذه.

```csharp
public RowCollection Rows { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRowsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // حدد عرض العمود وارتفاع الصف
            worksheet.Cells.SetColumnWidthPixel(0, 200);
            worksheet.Cells.Rows[0].Height = 50;
            
            // الوصول إلى خصائص الصف عبر مجموعة Rows
            Row row = worksheet.Cells.Rows[0];
            Console.WriteLine($"Row 0 height: {row.Height}");
            Console.WriteLine($"Is height matched: {row.IsHeightMatched}");
            
            // تعديل خصائص الصف
            row.IsHeightMatched = true;
            row.Height = 60;
            
            // تحقق من التغييرات
            Console.WriteLine($"Modified row 0 height: {worksheet.Cells.GetRowHeightPixel(0)}");
            Console.WriteLine($"Is height matched after change: {row.IsHeightMatched}");
            
            // احفظ المصنف
            workbook.Save("CellsPropertyRowsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


