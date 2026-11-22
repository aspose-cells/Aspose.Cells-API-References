---
title: "PageSetup.TopMarginInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل حجم الهامش العلوي بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/pagesetup/topmargininch/
---
## PageSetup.TopMarginInch property

يمثل حجم الهامش العلوي، بوحدة البوصة.

```csharp
public double TopMarginInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginInchDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // تعيين الهامش العلوي إلى 1.5 بوصة
            sheet.PageSetup.TopMarginInch = 1.5;

            // احصل على قيمة الهامش العلوي واطبعها
            Console.WriteLine("Top Margin (inches): " + sheet.PageSetup.TopMarginInch);

            // احفظ المصنف
            workbook.Save("PageSetup_TopMarginInch_Example.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


