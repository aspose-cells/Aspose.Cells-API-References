---
title: "Cells.SetRowHeightPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تضبط ارتفاع الصف بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells/cells/setrowheightpixel/
---
## Cells.SetRowHeightPixel method

يضبط ارتفاع الصف بوحدة البكسل.

```csharp
public void SetRowHeightPixel(int row, int pixels)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| بكسلات | Int32 | عدد البكسلات. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // اضبط ارتفاع الصف الأول إلى 50 بكسل
            worksheet.Cells.SetRowHeightPixel(0, 50);

            // اضبط ارتفاع الصف الثاني إلى 100 بكسل
            worksheet.Cells.SetRowHeightPixel(1, 100);

            // احفظ المصنف
            workbook.Save("RowHeightPixelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


