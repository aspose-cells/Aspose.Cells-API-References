---
title: "Cells.SetColumnWidthPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تضبط عرض العمود بوحدة البكسل في العرض العادي"
type: docs
url: /ar/net/aspose.cells/cells/setcolumnwidthpixel/
---
## Cells.SetColumnWidthPixel method

يضبط عرض العمود بوحدة البكسل في العرض العادي.

```csharp
public void SetColumnWidthPixel(int column, int pixels)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |
| بكسلات | Int32 | عدد البكسلات. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ضبط عرض الأعمدة بوحدات البكسل للأعمدة من 1 إلى 5
            for (int i = 0; i < 5; i++)
            {
                cells.SetColumnWidthPixel(i, 120); // 120 pixels width
            }

            // احفظ المصنف
            workbook.Save("SetColumnWidthPixelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


