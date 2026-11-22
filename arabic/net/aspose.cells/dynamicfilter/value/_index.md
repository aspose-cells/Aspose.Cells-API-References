---
title: "DynamicFilter.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DynamicFilter. تُرجع وتعيّن قيمة الفلتر الديناميكي"
type: docs
url: /ar/net/aspose.cells/dynamicfilter/value/
---
## DynamicFilter.Value property

يحصل ويضبط قيمة الفلتر الديناميكي.

```csharp
public object Value { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            // إنشاء مرشح تلقائي
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // اعرض قيمة الفلتر الحالية
            Console.WriteLine("Current DynamicFilter Value: " + filter.Value);

            // غيّر قيمة الفلتر لعرض تواريخ أبريل
            filter.Value = new DateTime(2023, 4, 1);
            filter.DynamicFilterType = DynamicFilterType.April;

            // تطبيق الفلتر
            worksheet.AutoFilter.Refresh();

            // حفظ النتيجة
            workbook.Save("DynamicFilterValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


