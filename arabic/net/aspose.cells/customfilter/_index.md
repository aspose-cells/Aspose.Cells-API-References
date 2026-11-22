---
title: "فئة CustomFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.CustomFilter class. يمثل الفلتر المخصص"
type: docs
url: /ar/net/aspose.cells/customfilter/
---
## CustomFilter class

يمثل الفلتر المخصص.

```csharp
public class CustomFilter
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Criteria](../../aspose.cells/customfilter/criteria/) { get; set; } | يحصل على المعايير ويضبطها. |
| [FilterOperatorType](../../aspose.cells/customfilter/filteroperatortype/) { get; set; } | يحصل على نوع عامل الفلتر ويضبطه. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetCriteria](../../aspose.cells/customfilter/setcriteria/)(FilterOperatorType, object) | يضبط معايير الفلتر. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCustomFilterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة بيانات عينة إلى ورقة العمل
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);

                // تطبيق الفلتر التلقائي على النطاق
                worksheet.AutoFilter.Range = "A1:A5";
                AutoFilter filter = worksheet.AutoFilter;

                // تطبيق فلتر مخصص للحصول على نسخة من CustomFilter
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // احصل على أول فلتر مخصص من مجموعة الفلاتر
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // عرض خصائص الفلتر
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // تعديل معايير الفلتر باستخدام طريقة SetCriteria
                customFilter.SetCriteria(FilterOperatorType.LessThan, 35);

                // عرض خصائص الفلتر المحدثة
                Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Updated Criteria Value: " + customFilter.Criteria);

                // احفظ المصنف
                workbook.Save("CustomFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CustomFilter: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


