---
title: "SheetRender.PageCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SheetRender. تحصل على العدد الإجمالي للصفحات في ورقة العمل الحالية"
type: docs
url: /ar/net/aspose.cells.rendering/sheetrender/pagecount/
---
## SheetRender.PageCount property

يحصل على إجمالي عدد الصفحات في ورقة العمل الحالية.

```csharp
public int PageCount { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Mary");
            cells["B3"].PutValue(25);
            cells["A4"].PutValue("Peter");
            cells["B4"].PutValue(35);

            // تعيين إعداد الصفحة للطباعة
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintArea = "A1:B4";
            pageSetup.FitToPagesTall = 1;
            pageSetup.FitToPagesWide = 1;

            // إنشاء SheetRender باستخدام الخيارات الافتراضية
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender render = new SheetRender(worksheet, options);

            // عرض عدد الصفحات
            Console.WriteLine("Page Count: " + render.PageCount);

            // تغيير إعداد الصفحة لإجبار وجود صفحات متعددة
            pageSetup.FitToPagesTall = 0;
            pageSetup.FitToPagesWide = 1;
            pageSetup.PrintArea = "A1:B100"; // Larger area than can fit on one page

            // إنشاء SheetRender جديد للحصول على عدد الصفحات المحدث
            SheetRender newRender = new SheetRender(worksheet, options);
            Console.WriteLine("Updated Page Count: " + newRender.PageCount);
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


