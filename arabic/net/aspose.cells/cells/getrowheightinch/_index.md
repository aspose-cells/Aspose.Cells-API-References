---
title: "Cells.GetRowHeightInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على ارتفاع صف محدد بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/cells/getrowheightinch/
---
## Cells.GetRowHeightInch method

يحصل على ارتفاع صف محدد بوحدة البوصة.

```csharp
public double GetRowHeightInch(int row)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف |

### قيمة الإرجاع

ارتفاع الصف

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين ارتفاع الصف بالبوصة للصف 5
            cells.SetRowHeightInch(5, 1.5);

            // الحصول على ارتفاع الصف بالبوصة للصف 5
            double rowHeight = cells.GetRowHeightInch(5);

            // أخرج النتيجة.
            Console.WriteLine("Row height in inches: " + rowHeight);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


