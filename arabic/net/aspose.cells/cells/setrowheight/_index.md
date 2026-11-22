---
title: "Cells.SetRowHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحدد ارتفاع الصف المحدد"
type: docs
url: /ar/net/aspose.cells/cells/setrowheight/
---
## Cells.SetRowHeight method

يضبط ارتفاع الصف المحدد.

```csharp
public void SetRowHeight(int row, double height)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| الارتفاع | Double | ارتفاع الصف. بوحدة النقطة يجب أن يكون بين 0 و 409.5. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // حدد ارتفاع الصف للصف الأول (المؤشر 0) إلى 25.5 نقطة
            cells.SetRowHeight(0, 25.5);

            // تحقق من ارتفاع الصف
            Console.WriteLine("Row height of row 0: " + cells.GetRowHeight(0));
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


