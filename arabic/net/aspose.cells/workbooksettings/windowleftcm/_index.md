---
title: "WorkbookSettings.WindowLeftCM"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. بوحدة السنتيمتر"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowleftcm/
---
## WorkbookSettings.WindowLeftCM property

المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. بوحدة السنتيمتر.

```csharp
public double WindowLeftCM { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftCMDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // ضبط خاصية WindowLeftCM (المسافة من الحافة اليسرى للشاشة بالسنتيمترات)
            settings.WindowLeftCM = 2.54; // 1 inch = 2.54 cm

            // تحقق من الإعداد بطباعته
            Console.WriteLine("WindowLeftCM: " + settings.WindowLeftCM);

            // احفظ المصنف
            workbook.Save("WindowLeftCMDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


