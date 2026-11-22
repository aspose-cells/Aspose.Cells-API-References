---
title: "PivotGlobalizationSettings.GetTextOfHours"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. تحصل على النص المحلي لساعات"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextofhours/
---
## PivotGlobalizationSettings.GetTextOfHours method

يحصل على النص المحلي لـ "Hours".

```csharp
public virtual string GetTextOfHours()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfHoursDemo
    {
        public static void Run()
        {
            // إنشاء كائن من PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // إظهار طريقة GetTextOfHours
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());

            // عرض إضافي للطرق المتعلقة بالوقت
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### انظر أيضًا

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


