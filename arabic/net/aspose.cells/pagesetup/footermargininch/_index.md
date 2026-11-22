---
title: "PageSetup.FooterMarginInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل المسافة من أسفل الصفحة إلى التذييل بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/pagesetup/footermargininch/
---
## PageSetup.FooterMarginInch property

يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة البوصات.

```csharp
public double FooterMarginInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginInchDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإعداداتها PageSetup
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // ضبط هامش التذييل بالبوصة
            pageSetup.FooterMarginInch = 0.5;
            
            // ضبط هوامش أخرى للعرض
            pageSetup.HeaderMarginInch = 0.3;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;
            
            // احفظ المصنف
            workbook.Save("PageSetupMargins.xlsx");
            
            // طباعة التأكيد
            Console.WriteLine("Footer margin set to: " + pageSetup.FooterMarginInch + " inches");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


