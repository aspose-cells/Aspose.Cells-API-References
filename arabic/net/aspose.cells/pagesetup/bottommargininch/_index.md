---
title: "PageSetup.BottomMarginInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل حجم الهامش السفلي بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/pagesetup/bottommargininch/
---
## PageSetup.BottomMarginInch property

يمثل حجم الهامش السفلي، بوحدة البوصة.

```csharp
public double BottomMarginInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginInchDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى PageSetup للورقة الأولى
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // تعيين هوامش مختلفة بالبوصة
            setup.HeaderMarginInch = 0.1;
            setup.FooterMarginInch = 0.2;
            setup.TopMarginInch = 0.3;
            setup.BottomMarginInch = 0.4; // Demonstrating BottomMarginInch property
            setup.LeftMarginInch = 0.5;
            setup.RightMarginInch = 0.6;
            
            // احفظ المصنف
            workbook.Save("PageMarginsDemo.xlsx");
            
            // اعرض التأكيد
            Console.WriteLine("Workbook saved with bottom margin set to: " + setup.BottomMarginInch + " inches");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


