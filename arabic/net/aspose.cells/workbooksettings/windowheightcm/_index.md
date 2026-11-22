---
title: "WorkbookSettings.WindowHeightCM"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. ارتفاع النافذة بوحدة السنتيمتر"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowheightcm/
---
## WorkbookSettings.WindowHeightCM property

ارتفاع النافذة، بوحدة السنتيمتر.

```csharp
public double WindowHeightCM { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightCMDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;

            // تعيين خاصية WindowHeightCM
            settings.WindowHeightCM = 15.5;

            // عرض القيمة المحددة
            Console.WriteLine("Window Height in Centimeters: " + settings.WindowHeightCM);

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


