---
title: "PageSetup.IsPercentScale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. إذا كانت هذه الخاصية False فإن خاصيتي FitToPagesWide و FitToPagesTall تتحكمان في كيفية تحجيم ورقة العمل"
type: docs
url: /ar/net/aspose.cells/pagesetup/ispercentscale/
---
## PageSetup.IsPercentScale property

إذا كانت هذه الخاصية خاطئة، فإن خاصيتي FitToPagesWide وFitToPagesTall تتحكمان في كيفية تحجيم الورقة.

```csharp
public bool IsPercentScale { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsPercentScaleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى PageSetup وتعيين التحجيم إلى 80% (نسبة مئوية)
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.Zoom = 80;
            pageSetup.IsPercentScale = true;

            // أخرج الإعدادات لتوضيح IsPercentScale
            Console.WriteLine("Zoom: " + pageSetup.Zoom);
            Console.WriteLine("IsPercentScale: " + pageSetup.IsPercentScale);

            // احفظ المصنف
            workbook.Save("PageSetup_IsPercentScale_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


