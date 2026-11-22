---
title: "WorkbookSettings.WindowHeightInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. ارتفاع النافذة بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowheightinch/
---
## WorkbookSettings.WindowHeightInch property

ارتفاع النافذة، بوحدة البوصة.

```csharp
public double WindowHeightInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightInchDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;

            // تعيين ارتفاع النافذة بالبوصة
            settings.WindowHeightInch = 5.5;

            // عرض ارتفاع النافذة بالبوصة
            Console.WriteLine("Window Height in Inches: " + settings.WindowHeightInch);

            // احفظ المصنف
            workbook.Save("WindowHeightInchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


