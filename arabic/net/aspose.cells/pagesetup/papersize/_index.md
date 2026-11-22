---
title: "PageSetup.PaperSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل حجم الورق"
type: docs
url: /ar/net/aspose.cells/pagesetup/papersize/
---
## PageSetup.PaperSize property

يمثل حجم الورق.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // تعيين حجم الورق إلى الظرف B6
            sheet.PageSetup.PaperSize = PaperSizeType.PaperEnvelopeB6;

            // طباعة حجم الورق الحالي
            Console.WriteLine("Current paper size: " + sheet.PageSetup.PaperSize);

            // احفظ المصنف
            workbook.Save("PageSetup_PaperSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


