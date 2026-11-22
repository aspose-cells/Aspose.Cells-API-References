---
title: "AbstractGlobalizationSettings.Compare"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractGlobalizationSettings. تقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة"
type: docs
url: /ar/net/aspose.cells/abstractglobalizationsettings/compare/
---
## AbstractGlobalizationSettings.Compare method

يقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة.

```csharp
public virtual int Compare(string v1, string v2, bool ignoreCase)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| v1 | String | السلسلة الأولى |
| v2 | String | السلسلة الثانية |
| ignoreCase | منطقي | ما إذا كان يجب تجاهل حالة الأحرف عند مقارنة القيم |

### قيمة الإرجاع

عدد صحيح يحدد العلاقة المعجمية بين المتقارنين

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractGlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء إعدادات تعميم مخصصة تتجاوز طريقة Compare
            var settings = new CustomGlobalizationSettings();
            
            // إنشاء مصنف بإعدادات تعميم مخصصة
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // تحضير السلاسل للمقارنة
            string string1 = "Apple";
            string string2 = "apple";
            bool ignoreCase = true;

            try
            {
                // ستُستدعى طريقة Compare داخليًا أثناء عمليات مثل الفرز
                // نوضح الاستخدام المباشر هنا
                int comparisonResult = settings.Compare(string1, string2, ignoreCase);
                
                Console.WriteLine($"Comparison result: {comparisonResult}");
                Console.WriteLine($"Strings compared: '{string1}' and '{string2}' (Ignore case: {ignoreCase})");

                // توضيح التأثير بفرز البيانات
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Orange");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Apple");

                // إنشاء DataSorter وتحديد النطاق للفرز
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Ascending);

                sorter.Sort(worksheet.Cells, 0, 0, 3, 0);
                workbook.Save("StringComparisonDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during string comparison: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return String.Compare(v1, v2, ignoreCase);
            }
        }
    }
}
```

### انظر أيضًا

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


