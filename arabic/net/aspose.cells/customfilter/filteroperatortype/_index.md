---
title: "CustomFilter.FilterOperatorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomFilter. تحصل وتعيّن نوع عامل التصفية"
type: docs
url: /ar/net/aspose.cells/customfilter/filteroperatortype/
---
## CustomFilter.FilterOperatorType property

يحصل على نوع عامل الفلتر ويضبطه.

```csharp
public FilterOperatorType FilterOperatorType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Mike");
            worksheet.Cells["A5"].PutValue("Emily");

            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // تطبيق مرشح مخصص باستخدام عامل Contains
            filter.Custom(0, FilterOperatorType.Contains, "e");
            
            // احصل على أول مرشح مخصص
            CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
            
            // عرض خاصية FilterOperatorType
            Console.WriteLine("Initial Filter Operator: " + customFilter.FilterOperatorType);
            Console.WriteLine("Criteria: " + customFilter.Criteria);
            
            // تغيير نوع عامل التصفية
            customFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
            
            // احفظ المصنف
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


