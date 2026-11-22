---
title: "PageSetup.HeaderMargin"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل المسافة من أعلى الصفحة إلى الرأس بوحدة السنتيمترات"
type: docs
url: /ar/net/aspose.cells/pagesetup/headermargin/
---
## PageSetup.HeaderMargin property

يمثل المسافة من أعلى الصفحة إلى الترويسة، بوحدة السنتيمترات.

```csharp
public double HeaderMargin { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // ضبط هامش الرأس بالسنتيمترات
            pageSetup.HeaderMargin = 1.5;

            // تحقق من ضبط هامش الرأس
            Console.WriteLine("Header Margin: " + pageSetup.HeaderMargin + " cm");

            // احفظ المصنف
            workbook.Save("HeaderMarginDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


