---
title: "CustomFilter.SetCriteria"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomFilter. تعيين معايير التصفية"
type: docs
url: /ar/net/aspose.cells/customfilter/setcriteria/
---
## CustomFilter.SetCriteria method

يضبط معايير الفلتر.

```csharp
public void SetCriteria(FilterOperatorType filterOperator, object criteria)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filterOperator | FilterOperatorType | نوع عامل التصفية |
| معايير | Object | قيمة معايير التصفية |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterMethodSetCriteriaWithFilterOperatorTObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);

            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;

            try
            {
                // تطبيق فلتر مخصص للحصول على نسخة من CustomFilter
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // احصل على أول فلتر مخصص من مجموعة الفلاتر
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // تعيين المعايير باستخدام طريقة SetCriteria
                customFilter.SetCriteria(FilterOperatorType.GreaterThan, 25);

                // عرض المعايير المحددة
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // احفظ المصنف
                workbook.Save("SetCriteriaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


