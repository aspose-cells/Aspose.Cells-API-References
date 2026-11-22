---
title: "GlobalizationSettings.Compare"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/compare/
---
## GlobalizationSettings.Compare method

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

    public class GlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل باستخدام إعدادات العولمة المخصصة
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomComparisonSettings();

            try
            {
                // إظهار استخدام طريقة Compare مباشرة
                GlobalizationSettings settings = workbook.Settings.GlobalizationSettings;
                int result1 = settings.Compare("Apple", "apple", true);
                int result2 = settings.Compare("Apple", "apple", false);
                
                Console.WriteLine($"Case-insensitive comparison result: {result1}");
                Console.WriteLine($"Case-sensitive comparison result: {result2}");

                // إظهار التأثير على عمليات جدول البيانات
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Banana");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Cherry");

                // فرز البيانات باستخدام مقارنة مخصصة
                DataSorter sorter = workbook.DataSorter;
                sorter.Order1 = SortOrder.Ascending;
                sorter.Key1 = 0;
                sorter.Sort(worksheet.Cells, 0, 0, 2, 0); // Corrected range to rows 0-2

                Console.WriteLine("Sorted data with custom comparison rules:");
                for (int row = 0; row < 3; row++)
                {
                    Cell cell = worksheet.Cells[row, 0];
                    Console.WriteLine(cell.StringValue);
                }

                workbook.Save("GlobalizationCompareDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomComparisonSettings : GlobalizationSettings
    {
        public override int Compare(string v1, string v2, bool ignoreCase)
        {
            // تنفيذ منطق مقارنة مخصص
            var comparison = ignoreCase ? 
                StringComparison.OrdinalIgnoreCase : 
                StringComparison.Ordinal;
            
            return string.Compare(v1?.Trim() ?? "", v2?.Trim() ?? "", comparison);
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


