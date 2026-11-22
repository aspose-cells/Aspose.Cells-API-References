---
title: "AbstractGlobalizationSettings.GetCollationKey"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractGlobalizationSettings. تحول السلسلة إلى كائن قابل للمقارنة وفقًا لقواعد ترتيب معينة"
type: docs
url: /ar/net/aspose.cells/abstractglobalizationsettings/getcollationkey/
---
## AbstractGlobalizationSettings.GetCollationKey method

يحوّل النص إلى كائن قابل للمقارنة وفقًا لقواعد ترتيب معينة.

```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| v | String | يجب مقارنة قيمة السلسلة مع القيم الأخرى. |
| ignoreCase | منطقي | ما إذا كان يجب تجاهل حالة الأحرف عند مقارنة القيم |

### قيمة الإرجاع

يمكن استخدام الكائن لمقارنة أو فرز قيم السلاسل

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractGlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء إعدادات تعميم مخصصة تتجاوز طريقة GetCollationKey
            var settings = new CustomGlobalizationSettings();
            
            // إنشاء مصنف بإعدادات تعميم مخصصة
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // تحضير السلسلة لمفتاح الترتيب
            string inputString = "Sample Text";
            bool ignoreCase = true;

            try
            {
                // استدعاء GetCollationKey مباشرةً
                IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
                
                Console.WriteLine($"Original string: {inputString}");
                Console.WriteLine($"Collation key: {collationKey}");
                Console.WriteLine($"Ignore case: {ignoreCase}");

                // توضيح التأثير باستخدامه في عمليات ورقة العمل
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // سيستخدم الفرز GetCollationKey داخليًا
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Descending);

                sorter.Sort(worksheet.Cells, 0, 0, 2, 0);
                
                workbook.Save("GetCollationKeyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during GetCollationKey operation: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }

    }
}
```

### انظر أيضًا

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


