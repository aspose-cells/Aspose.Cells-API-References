---
title: "Workbook.Theme"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تُجلب اسم السمة"
type: docs
url: /ar/net/aspose.cells/workbook/theme/
---
## Workbook.Theme property

يحصل على اسم السمة.

```csharp
public string Theme { get; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyThemeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // عرض الحصول على السمة الافتراضية
            Console.WriteLine("Default theme: " + workbook.Theme);
            
            // تغيير لون السمة والتحقق منه
            workbook.SetThemeColor(ThemeColorType.Accent1, Color.Blue);
            Color accent1 = workbook.GetThemeColor(ThemeColorType.Accent1);
            Console.WriteLine("Modified Accent1 color: " + accent1);
            
            // حفظ دفتر العمل لعرض استمرارية السمة
            workbook.Save("ThemeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


