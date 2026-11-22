---
title: "PivotGlobalizationSettings.GetNameOfDataField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. تحصل على اسم العرض لحقل محور البيانات. التنسيق الافتراضي هو Sum Of Field"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/
---
## PivotGlobalizationSettings.GetNameOfDataField method

يحصل على اسم العرض لحقل بيانات المحور. التنسيق الافتراضي هو "Sum Of Field".

```csharp
public virtual string GetNameOfDataField(ConsolidationFunction function, string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دالة | ConsolidationFunction | تُستخدم الدالة لتلخيص قيم حقل المحور. |
| name | String | الاسم الأصلي لحقل المحور. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetNameOfDataFieldWithConsolidationFuStringDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء كائن من PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // حدد المعلمات لطريقة GetNameOfDataField
                ConsolidationFunction function = ConsolidationFunction.Sum;
                string fieldName = "Sales";

                // استدعِ طريقة GetNameOfDataField
                string result = globalizationSettings.GetNameOfDataField(function, fieldName);

                // أخرج النتيجة.
                Console.WriteLine($"Localized name for data field '{fieldName}' with function '{function}': {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNameOfDataField: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


