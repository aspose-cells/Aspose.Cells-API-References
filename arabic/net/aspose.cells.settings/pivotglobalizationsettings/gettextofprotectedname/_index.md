---
title: "PivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. تحصل على النص للاسم المحمي المحدد"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/
---
## PivotGlobalizationSettings.GetTextOfProtectedName method

يحصل على النص لاسم محمي محدد.

```csharp
public virtual string GetTextOfProtectedName(string protectedName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| protectedName | String | الاسم المحمي في PivotTable. |

### قيمة الإرجاع

الأسماء المحمية المحلية في PivotTable.

### ملاحظات

في برنامج Ms Excel، بعض الأسماء غير مسموح باستخدامها كاسم لحقول PivotFields في PivotTable. تختلف هذه الأسماء حسب المنطقة، ويمكن للمستخدم تحديدها صراحةً وفقًا للمنطقة المستخدمة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectedNameWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء كائن من PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // حدد اسمًا محميًا لاسترجاع نصه
                string protectedName = "SensitiveData";

                // استدعِ طريقة GetTextOfProtectedName
                string result = globalizationSettings.GetTextOfProtectedName(protectedName);

                // أخرج النتيجة.
                Console.WriteLine($"Text for protected name \"{protectedName}\": {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


