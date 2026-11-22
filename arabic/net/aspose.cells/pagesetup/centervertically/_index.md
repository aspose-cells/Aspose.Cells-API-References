---
title: "PageSetup.CenterVertically"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل ما إذا كان الورق يُطبع مركّزًا عموديًا"
type: docs
url: /ar/net/aspose.cells/pagesetup/centervertically/
---
## PageSetup.CenterVertically property

يمثل ما إذا كانت الورقة تُطبع مركزة عمودياً.

```csharp
public bool CenterVertically { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterVerticallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى PageSetup وتعيين CenterVertically
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.CenterVertically = true;
            
            // إضافة بعض البيانات التجريبية لتصوّر التأثير
            worksheet.Cells["A1"].PutValue("This worksheet content will be centered vertically when printed");
            worksheet.Cells["A2"].PutValue("CenterVertically = true");
            
            // احفظ المصنف
            workbook.Save("PageSetup_CenterVertically.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


