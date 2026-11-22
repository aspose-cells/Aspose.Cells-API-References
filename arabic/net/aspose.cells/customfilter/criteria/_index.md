---
title: "CustomFilter.Criteria"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomFilter. تحصل وتعيّن المعايير"
type: docs
url: /ar/net/aspose.cells/customfilter/criteria/
---
## CustomFilter.Criteria property

يحصل على المعايير ويضبطها.

```csharp
public object Criteria { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Numbers");
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(5);
            worksheet.Cells["A5"].PutValue(9);
            worksheet.Cells["A6"].PutValue(3);

            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:A6";
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // إضافة مرشح مخصص
            int fieldIndex = 0;
            autoFilter.Custom(fieldIndex, FilterOperatorType.GreaterOrEqual, 5);
            
            // احصل على عمود التصفية وعرض المعايير
            FilterColumn fc = autoFilter.FilterColumns[fieldIndex];
            CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
            Console.WriteLine("Filter Criteria: " + cf.Criteria);
            
            // تحديث الفلتر
            autoFilter.Refresh();
            
            // احفظ المصنف
            workbook.Save("CustomFilterExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


