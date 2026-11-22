---
title: "PageSetup.FooterMargin"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل المسافة من أسفل الصفحة إلى التذييل بوحدة السنتيمتر"
type: docs
url: /ar/net/aspose.cells/pagesetup/footermargin/
---
## PageSetup.FooterMargin property

يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة السنتيمترات.

```csharp
public double FooterMargin { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // عيّن هامش التذييل بالسنتيمترات
            pageSetup.FooterMargin = 1.5;

            // أضف بعض المحتوى لرؤية التأثير
            worksheet.Cells["A1"].PutValue("Footer Margin Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates setting footer margin to 1.5 cm");

            // عيّن نص التذييل لجعل الهامش مرئيًا
            pageSetup.SetFooter(0, "&A - Footer text to demonstrate margin");

            // احفظ المصنف
            workbook.Save("FooterMarginDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


