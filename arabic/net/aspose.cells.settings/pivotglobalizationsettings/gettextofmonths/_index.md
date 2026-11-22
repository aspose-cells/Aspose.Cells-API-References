---
title: "PivotGlobalizationSettings.GetTextOfMonths"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. تحصل على النص المحلي للأشهر"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/
---
## PivotGlobalizationSettings.GetTextOfMonths method

يحصل على النص المحلي لـ "Months".

```csharp
public virtual string GetTextOfMonths()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMonthsDemo
    {
        public static void Run()
        {
            // إنشاء إعدادات تعميم مخصصة
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // عرض GetTextOfMonths
            Console.WriteLine("Custom Months Text: " + customSettings.GetTextOfMonths());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfMonths()
        {
            // إرجاع نص مخصص مُعرب لـ "Months"
            return "Custom Months Label";
        }
    }
}
```

### انظر أيضًا

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


