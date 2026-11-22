---
title: "PageSetup.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تنسخ إعدادات إعداد الصفحة"
type: docs
url: /ar/net/aspose.cells/pagesetup/copy/
---
## PageSetup.Copy method

ينسخ إعدادات إعداد الصفحة.

```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | PageSetup | المصدر. |
| copyOptions | CopyOptions | خيارات النسخ. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCopyWithPageSetupCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // عيّن خصائص PageSetup للورقة الأولى
            workbook.Worksheets[0].PageSetup.PaperSize = PaperSizeType.PaperA3;
            
            // انسخ PageSetup من الورقة الأولى إلى الورقة الثانية باستخدام CopyOptions
            workbook.Worksheets[1].PageSetup.Copy(workbook.Worksheets[0].PageSetup, new CopyOptions());
            
            Console.WriteLine("Paper size of second worksheet: " + workbook.Worksheets[1].PageSetup.PaperSize);
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


