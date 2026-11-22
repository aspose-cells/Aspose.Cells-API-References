---
title: "PageSetup.HeaderMarginInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل المسافة من أعلى الصفحة إلى الرأس بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/pagesetup/headermargininch/
---
## PageSetup.HeaderMarginInch property

يمثل المسافة من أعلى الصفحة إلى الترويسة، بوحدة البوصات.

```csharp
public double HeaderMarginInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginInchDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإلى خاصية PageSetup الخاصة بها
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // تعيين هامش الرأس بالبوصة
            pageSetup.HeaderMarginInch = 0.5;
            
            // ضبط هوامش أخرى للعرض
            pageSetup.FooterMarginInch = 0.25;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;

            // احفظ المصنف
            workbook.Save("PageSetupMargins.xlsx");

            // عرض قيمة هامش الرأس
            Console.WriteLine("Header Margin (inches): " + pageSetup.HeaderMarginInch);
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


