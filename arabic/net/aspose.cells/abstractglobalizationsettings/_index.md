---
title: "فئة AbstractGlobalizationSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.AbstractGlobalizationSettings. تمثل إعدادات العولمة"
type: docs
url: /ar/net/aspose.cells/abstractglobalizationsettings/
---
## AbstractGlobalizationSettings class

يمثل إعدادات العولمة.

```csharp
public abstract class AbstractGlobalizationSettings
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare/)(string, string, bool) | يقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة. |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey/)(string, bool) | يحوّل النص إلى كائن قابل للمقارنة وفقًا لقواعد ترتيب معينة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAbstractGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // إنشاء تنفيذ مخصص لـ AbstractGlobalizationSettings
            var customSettings = new CustomGlobalizationSettings();

            try
            {
                // عرض طريقة Compare
                string str1 = "Hello";
                string str2 = "hello";
                bool ignoreCase = true;

                int comparisonResult = customSettings.Compare(str1, str2, ignoreCase);
                Console.WriteLine($"Comparison result ({str1} vs {str2}, ignoreCase={ignoreCase}): {comparisonResult}");

                // عرض طريقة GetCollationKey
                string testString = "Sample";
                IComparable collationKey = customSettings.GetCollationKey(testString, ignoreCase);
                Console.WriteLine($"Collation key for '{testString}' (ignoreCase={ignoreCase}): {collationKey}");

                // تطبيق الإعدادات على مصنف
                Workbook workbook = new Workbook();
                workbook.Settings.GlobalizationSettings = customSettings;

                // إضافة بعض البيانات لعرض الإعدادات قيد التنفيذ
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // احفظ المصنف
                workbook.Save("GlobalizationSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved with custom globalization settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return string.Compare(v1, v2, ignoreCase ? StringComparison.OrdinalIgnoreCase : StringComparison.Ordinal);
            }

            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


