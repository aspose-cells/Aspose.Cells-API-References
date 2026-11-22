---
title: "Cells.GetViewColumnWidthPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. الحصول على العرض في نوع عرض مختلف"
type: docs
url: /ar/net/aspose.cells/cells/getviewcolumnwidthpixel/
---
## Cells.GetViewColumnWidthPixel method

احصل على العرض في نوع عرض مختلف.

```csharp
public int GetViewColumnWidthPixel(int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |

### قيمة الإرجاع

عرض العمود بوحدة البكسل

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين نوع العرض إلى PageLayoutView
            worksheet.ViewType = ViewType.PageLayoutView;
            
            // تعيين عرض العمود بالأحرف (سيتم تحويله إلى بكسلات)
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // احصل على عرض العمود بالبكسل
            int columnWidthInPixels = worksheet.Cells.GetViewColumnWidthPixel(0);
            
            // أخرج النتيجة.
            Console.WriteLine("Column width in pixels: " + columnWidthInPixels);
            
            // احفظ المصنف
            workbook.Save("ColumnWidthTest.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


