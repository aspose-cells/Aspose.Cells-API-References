---
title: "PageSetup.PrintGridlines"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل ما إذا كانت خطوط الشبكة الخلوية تُطبع على الصفحة"
type: docs
url: /ar/net/aspose.cells/pagesetup/printgridlines/
---
## PageSetup.PrintGridlines property

يمثل ما إذا كانت خطوط شبكة الخلايا تُطبع على الصفحة.

```csharp
public bool PrintGridlines { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintGridlinesDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // وضع بيانات تجريبية في الخلية
            worksheet.Cells["A1"].PutValue("PrintGridlines Property Demo");
            worksheet.Cells["A3"].PutValue("Gridlines will ");
            worksheet.Cells["B3"].PutValue(worksheet.PageSetup.PrintGridlines ? "appear" : "not appear");
            worksheet.Cells["A4"].PutValue("when printing this sheet.");

            // تبديل خاصية PrintGridlines
            worksheet.PageSetup.PrintGridlines = true;
            
            // احفظ المصنف
            workbook.Save("PrintGridlinesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


