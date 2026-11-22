---
title: "WorkbookSettings.WindowTopCM"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. المسافة من الحافة العليا لمنطقة العميل إلى الحافة العليا للنافذة بوحدة السنتيمتر"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowtopcm/
---
## WorkbookSettings.WindowTopCM property

المسافة من الحافة العليا لمنطقة العميل إلى الحافة العليا للنافذة، بوحدة السنتيمتر.

```csharp
public double WindowTopCM { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopCMDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;

            // تعيين خاصية WindowTopCM (الموضع من الأعلى بالسنتيمترات)
            settings.WindowTopCM = 2.5;

            // عرض قيمة WindowTopCM الحالية
            Console.WriteLine("Window Top Position (cm): " + settings.WindowTopCM);

            // احفظ المصنف
            workbook.Save("WindowTopCMDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


