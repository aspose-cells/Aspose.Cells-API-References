---
title: "WorkbookSettings.WindowWidthInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. عرض النافذة بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowwidthinch/
---
## WorkbookSettings.WindowWidthInch property

عرض النافذة، بوحدة البوصة.

```csharp
public double WindowWidthInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthInchDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;

            // ضبط عرض النافذة بالبوصة
            settings.WindowWidthInch = 10.5;

            // عرض عرض النافذة بالبوصة
            Console.WriteLine("Window Width in Inches: " + settings.WindowWidthInch);

            // احفظ المصنف
            workbook.Save("WindowWidthInchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


