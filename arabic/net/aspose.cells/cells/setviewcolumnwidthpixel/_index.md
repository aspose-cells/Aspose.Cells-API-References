---
title: "Cells.SetViewColumnWidthPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تعيين عرض العمود في عرض مختلف"
type: docs
url: /ar/net/aspose.cells/cells/setviewcolumnwidthpixel/
---
## Cells.SetViewColumnWidthPixel method

يضبط عرض العمود في عرض مختلف.

```csharp
public void SetViewColumnWidthPixel(int column, int pixels)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |
| بكسلات | Int32 | العرض بوحدة البكسل. |

### ملاحظات

إذا كان نوع العرض الحالي هو PageLayoutView، فإن عرض العمود يكون نفسه عرض الطباعة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetViewColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // تعيين بيانات عينة
            sheet.Cells[0, 0].Value = "Sample Text";

            // حساب عرض البكسل (100 بكسل في هذا المثال)
            int pixelWidth = 100;

            // تعيين عرض العمود بالبكسل
            sheet.Cells.SetViewColumnWidthPixel(0, pixelWidth);

            // احفظ المصنف
            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


