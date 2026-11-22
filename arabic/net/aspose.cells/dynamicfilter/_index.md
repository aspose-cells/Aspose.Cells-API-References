---
title: "فئة DynamicFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.DynamicFilter. تمثل الفلتر الديناميكي"
type: docs
url: /ar/net/aspose.cells/dynamicfilter/
---
## DynamicFilter class

يمثل الفلتر الديناميكي.

```csharp
public class DynamicFilter
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DynamicFilterType](../../aspose.cells/dynamicfilter/dynamicfiltertype/) { get; set; } | يحصل ويضبط نوع هذا الفلتر الديناميكي. |
| [MaxValue](../../aspose.cells/dynamicfilter/maxvalue/) { get; set; } | يحصل ويضبط القيمة القصوى للفلتر الديناميكي. |
| [Value](../../aspose.cells/dynamicfilter/value/) { get; set; } | يحصل ويضبط قيمة الفلتر الديناميكي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء مصنف وورقة عمل (اختياري للسياق)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Name = "DemoSheet";

                // ملء بعض البيانات الرقمية النموذجية
                worksheet.Cells["A1"].PutValue("Numbers");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);
                worksheet.Cells["A6"].PutValue(50);

                // تحديد نطاق الفلتر التلقائي
                worksheet.AutoFilter.Range = "A1:A6";

                // تطبيق فلتر ديناميكي (AboveAverage) على العمود الأول
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);

                // استرجاع كائن DynamicFilter الذي تم إنشاؤه بواسطة AutoFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // قم بتعيين الخصائص الإضافية إذا رغبت
                filter.Value = 25;      // Example custom value
                filter.MaxValue = 45;   // Example max value

                // اعرض الخصائص المحددة
                Console.WriteLine($"DynamicFilterType: {filter.DynamicFilterType}");
                Console.WriteLine($"Value: {filter.Value}");
                Console.WriteLine($"MaxValue: {filter.MaxValue}");

                // قم بتحديث الفلتر لتطبيق التغييرات
                worksheet.AutoFilter.Refresh();

                // احفظ المصنف (سيتم حفظ البيانات المصفاة)
                workbook.Save("DynamicFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DynamicFilter: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


