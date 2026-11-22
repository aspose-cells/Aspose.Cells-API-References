---
title: "Worksheet.GetAdvancedFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تحصل على إعدادات الفلتر المتقدم"
type: docs
url: /ar/net/aspose.cells/worksheet/getadvancedfilter/
---
## Worksheet.GetAdvancedFilter method

يحصل على إعدادات الفلتر المتقدم.

```csharp
public AdvancedFilter GetAdvancedFilter()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetAdvancedFilterDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إعداد البيانات للتصفية
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Alice");
            sheet.Cells["A4"].PutValue("Bob");
            
            // إعداد نطاق المعايير
            sheet.Cells["C1"].PutValue("Name");
            sheet.Cells["C2"].PutValue("John");
            
            // تطبيق الفلتر المتقدم
            sheet.AdvancedFilter(true, "A1:A4", "C1:C2", "E1", false);
            
            // الحصول على الفلتر المتقدم
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            
            // إخراج نطاقات الفلتر
            Console.WriteLine("List Range: " + filter.ListRange);
            Console.WriteLine("Criteria Range: " + filter.CriteriaRange);
            Console.WriteLine("Copy To Range: " + filter.CopyToRange);
        }
    }
}
```

### انظر أيضًا

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


