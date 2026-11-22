---
title: "WorkbookSettings.WindowHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. ارتفاع النافذة بوحدة النقطة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowheight/
---
## WorkbookSettings.WindowHeight property

ارتفاع النافذة، بوحدة النقطة.

```csharp
public double WindowHeight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // تعيين خاصية WindowHeight
            settings.WindowHeight = 600;
            
            // تحقق من قيمة WindowHeight
            Console.WriteLine("Window Height set to: " + settings.WindowHeight);
            
            // احفظ المصنف
            workbook.Save("WindowHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


