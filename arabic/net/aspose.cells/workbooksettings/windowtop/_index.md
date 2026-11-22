---
title: "WorkbookSettings.WindowTop"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة بوحدة النقطة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowtop/
---
## WorkbookSettings.WindowTop property

المسافة من الحافة العليا لمنطقة العميل إلى الحافة العليا للنافذة، بوحدة النقطة.

```csharp
public double WindowTop { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // ضبط خاصية WindowTop لتحديد موضع النافذة على بعد 100 بكسل من الأعلى
            settings.WindowTop = 100;
            
            // تحقق من قيمة WindowTop
            Console.WriteLine("Window top position set to: " + settings.WindowTop);

            // احفظ المصنف
            workbook.Save("WindowTopDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


