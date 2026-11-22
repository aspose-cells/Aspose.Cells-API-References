---
title: "PageSetup.BlackAndWhite"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل ما إذا كانت عناصر المستند ستُطبع بالأبيض والأسود"
type: docs
url: /ar/net/aspose.cells/pagesetup/blackandwhite/
---
## PageSetup.BlackAndWhite property

يمثل ما إذا كانت عناصر المستند ستُطبع بالأبيض والأسود.

```csharp
public bool BlackAndWhite { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBlackAndWhiteDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على كائن PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // تعيين خاصية BlackAndWhite إلى true
            pageSetup.BlackAndWhite = true;
            Console.WriteLine("BlackAndWhite set to: " + pageSetup.BlackAndWhite);

            // تغيير خاصية BlackAndWhite إلى false
            pageSetup.BlackAndWhite = false;
            Console.WriteLine("BlackAndWhite changed to: " + pageSetup.BlackAndWhite);

            // احفظ المصنف
            workbook.Save("PageSetupBlackAndWhiteDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


