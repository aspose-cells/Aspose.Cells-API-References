---
title: "WorkbookSettings.WindowWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. عرض النافذة بوحدة النقطة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowwidth/
---
## WorkbookSettings.WindowWidth property

عرض النافذة، بوحدة النقطة.

```csharp
public double WindowWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // تعيين خاصية WindowWidth
            settings.WindowWidth = 800;
            
            // تحقق من قيمة WindowWidth
            Console.WriteLine("Window Width set to: " + settings.WindowWidth);
            
            // احفظ المصنف
            workbook.Save("WindowWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


