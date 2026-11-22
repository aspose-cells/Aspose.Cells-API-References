---
title: "PageSetup.CustomPaperSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تقوم بتعيين حجم ورق مخصص بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/pagesetup/custompapersize/
---
## PageSetup.CustomPaperSize method

يضبط حجم الورق المخصص، بوحدة البوصة.

```csharp
public void CustomPaperSize(double width, double height)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| العرض | Double | عرض الورق. |
| الارتفاع | Double | ارتفاع الورق. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCustomPaperSizeWithDoubleDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين حجم ورق مخصص (العرض: 1.5 بوصة، الارتفاع: 1.5 بوصة)
            worksheet.PageSetup.CustomPaperSize(1.5, 1.5);
            
            // احفظ المصنف لتوضيح التأثير
            workbook.Save("CustomPaperSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


