---
title: "WorkbookSettings.WindowTopInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. المسافة من الحافة العليا لمنطقة العميل إلى الحافة العليا للنافذة بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/windowtopinch/
---
## WorkbookSettings.WindowTopInch property

المسافة من الحافة العليا لمنطقة العميل إلى الحافة العليا للنافذة، بوحدة البوصة.

```csharp
public double WindowTopInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopInchDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // تعيين خاصية WindowTopInch لتحديد موضع النافذة على بعد 2 بوصة من الأعلى
            settings.WindowTopInch = 2.0;

            // تحقق من الإعداد بطباعته
            Console.WriteLine("Window top position (inches): " + settings.WindowTopInch);

            // احفظ المصنف
            workbook.Save("WindowTopInchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


