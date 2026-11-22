---
title: "PageSetup.PrintDraft"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل ما إذا كان سيتم طباعة الورقة بدون رسومات"
type: docs
url: /ar/net/aspose.cells/pagesetup/printdraft/
---
## PageSetup.PrintDraft property

يمثل ما إذا كانت الورقة ستُطبع بدون رسومات.

```csharp
public bool PrintDraft { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintDraftDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى كائن PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // تعيين خاصية PrintDraft إلى true
            pageSetup.PrintDraft = true;
            Console.WriteLine("PrintDraft set to: " + pageSetup.PrintDraft);

            // تغيير خاصية PrintDraft إلى false
            pageSetup.PrintDraft = false;
            Console.WriteLine("PrintDraft changed to: " + pageSetup.PrintDraft);

            // احفظ المصنف
            workbook.Save("PageSetup_PrintDraft_Example.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


