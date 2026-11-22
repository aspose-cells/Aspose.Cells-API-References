---
title: "PivotGlobalizationSettings.GetTextOfMinutes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. تحصل على النص المحلي للدقائق"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/
---
## PivotGlobalizationSettings.GetTextOfMinutes method

يحصل على النص المحلي لـ "Minutes".

```csharp
public virtual string GetTextOfMinutes()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMinutesDemo
    {
        public static void Run()
        {
            // إنشاء كائن من PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // عرض طريقة GetTextOfMinutes
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());

            // عرض إضافي للطرق الزمنية ذات الصلة للسياق
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### انظر أيضًا

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


