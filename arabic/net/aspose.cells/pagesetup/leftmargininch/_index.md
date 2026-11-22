---
title: "PageSetup.LeftMarginInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل حجم الهامش الأيسر بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/pagesetup/leftmargininch/
---
## PageSetup.LeftMarginInch property

يمثل حجم الهامش الأيسر، بوحدة البوصات.

```csharp
public double LeftMarginInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginInchDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // عيّن الهامش الأيسر بالبوصة (0.39 بوصة ≈ 1 سم)
            pageSetup.LeftMarginInch = 0.39;

            // أضف بعض البيانات لتوضيح الهامش
            worksheet.Cells["A1"].PutValue("Left Margin Demonstration");
            worksheet.Cells["A2"].PutValue("Left margin set to 0.39 inches");

            // احفظ المصنف
            workbook.Save("LeftMarginInchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


