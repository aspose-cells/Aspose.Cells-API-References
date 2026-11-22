---
title: "PageSetup.IsHFAlignMargins"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تشير إلى ما إذا كانت هوامش الرأس والتذييل محاذاة مع هوامش الصفحة. إذا كانت هذه الخاصية true فسيتم محاذاة رأس وتذييل اليسار مع الهامش الأيسر ورأس وتذييل اليمين مع الهامش الأيمن. هذا الخيار مفعّل بشكل افتراضي"
type: docs
url: /ar/net/aspose.cells/pagesetup/ishfalignmargins/
---
## PageSetup.IsHFAlignMargins property

يشير إلى ما إذا كانت هوامش الترويسة والتذييل متراصة مع هوامش الصفحة. إذا كانت هذه الخاصية صحيحة، سيتم محاذاة الترويسة والتذييل اليساريين مع الهامش الأيسر، والترويسة والتذييل اليمينيين مع الهامش الأيمن. يتم تمكين هذا الخيار افتراضيًا.

```csharp
public bool IsHFAlignMargins { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFAlignMarginsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // ضبط IsHFAlignMargins إلى true
            pageSetup.IsHFAlignMargins = true;
            Console.WriteLine("IsHFAlignMargins set to: " + pageSetup.IsHFAlignMargins);

            // تغيير IsHFAlignMargins إلى false
            pageSetup.IsHFAlignMargins = false;
            Console.WriteLine("IsHFAlignMargins changed to: " + pageSetup.IsHFAlignMargins);

            // احفظ المصنف
            workbook.Save("PageSetup_IsHFAlignMargins_Example.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


