---
title: "PivotGlobalizationSettings.GetTextOfQuarters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. احصل على النص المحلي للربع"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/
---
## PivotGlobalizationSettings.GetTextOfQuarters method

احصل على النص المحلي لـ "Quarters".

```csharp
public virtual string GetTextOfQuarters()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfQuartersDemo
    {
        public static void Run()
        {
            // إنشاء مثال لإعدادات العولمة
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // توضيح طريقة GetTextOfQuarters
            Console.WriteLine("Quarter labels: " + globalizationSettings.GetTextOfQuarters());
            
            // عرض تسميات الفترات الزمنية المرتبطة الأخرى للسياق
            Console.WriteLine("Year labels: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Month labels: " + globalizationSettings.GetTextOfMonths());
        }
    }
}
```

### انظر أيضًا

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


