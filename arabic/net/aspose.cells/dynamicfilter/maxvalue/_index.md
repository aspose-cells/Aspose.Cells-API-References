---
title: "DynamicFilter.MaxValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DynamicFilter. تحصل وتعيّن القيمة القصوى للمرشح الديناميكي"
type: docs
url: /ar/net/aspose.cells/dynamicfilter/maxvalue/
---
## DynamicFilter.MaxValue property

يحصل ويضبط القيمة القصوى للفلتر الديناميكي.

```csharp
public object MaxValue { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyMaxValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات رقمية نموذجية
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);

            // إنشاء مرشح تلقائي
            worksheet.AutoFilter.Range = "A1:A6";
            
            // طبق مرشحًا ديناميكيًا بمعايير النطاق
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // اعرض القيمة القصوى الحالية
            Console.WriteLine("Current MaxValue: " + filter.MaxValue);

            // نظرًا لعدم وجود DynamicFilterType.Between، سنستخدم نهجًا مختلفًا
            // على سبيل المثال، يمكننا استخدام مرشح مخصص بدلاً من ذلك
            worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, 20);
            worksheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, 40);

            // تطبيق الفلتر
            worksheet.AutoFilter.Refresh();

            // حفظ النتيجة
            workbook.Save("DynamicFilterMaxValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


