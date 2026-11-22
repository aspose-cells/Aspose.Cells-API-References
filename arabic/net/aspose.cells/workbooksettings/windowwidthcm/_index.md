---
title: "WorkbookSettings.WindowWidthCM"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. عرض النافذة بوحدة السنتيمتر"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowwidthcm/
---
## WorkbookSettings.WindowWidthCM property

عرض النافذة، بوحدة السنتيمتر.

```csharp
public double WindowWidthCM { get; set; }
```

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthCMDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // تعيين خاصية WindowWidthCM (20.32 سم = ~8 بوصات)
            settings.WindowWidthCM = 20.32;
            
            // تحقق من الإعداد بطباعته
            Console.WriteLine("Window Width in Centimeters: " + settings.WindowWidthCM);
            
            // احفظ المصنف
            workbook.Save("WindowWidthCMDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


