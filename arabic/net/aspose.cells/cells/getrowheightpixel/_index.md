---
title: "Cells.GetRowHeightPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على ارتفاع صف محدد بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells/cells/getrowheightpixel/
---
## Cells.GetRowHeightPixel method

يحصل على ارتفاع الصف المحدد بوحدة البكسل.

```csharp
public int GetRowHeightPixel(int row)
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
    public class CellsMethodGetRowHeightPixelWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء كائن Workbook جديد
            Workbook wb = new Workbook();

            // احصل على ورقة العمل الأولى
            Worksheet worksheet = wb.Worksheets[0];

            // تعيين ارتفاع الصف للصف 5 (بالبكسل)
            worksheet.Cells.SetRowHeightPixel(5, 30);

            // الحصول على ارتفاع الصف للصف 5 (بالبكسل)
            int rowHeight = worksheet.Cells.GetRowHeightPixel(5);

            Console.WriteLine("Row height of row 5 in pixels: " + rowHeight);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


