---
title: "PivotFilter.FilterType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFilter. تحصل على نوع الفلتر لمرشح المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfilter/filtertype/
---
## PivotFilter.FilterType property

يحصل على نوع المرشح لمرشح المحور.

```csharp
public PivotFilterType FilterType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى ورقة العمل الأولى وجدول محوري
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // تطبيق فلتر قيمة (أقل من 2) على الحقل الأساسي الأول
            pivotTable.BaseFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 2, 0);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // إعادة تحميل المصنف للتحقق من الفلتر
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            PivotTable verifyPivotTable = verifyWorkbook.Worksheets[0].PivotTables[0];
            
            // احصل على الفلتر المطبق وعرض خاصية FilterType
            PivotFilter filter = verifyPivotTable.BaseFields[0].GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType); // Should output ValueLessThan
            Console.WriteLine("Filter Value: " + filter.GetNumberValues()[0]); // Should output 2
        }
    }
}
```

### انظر أيضًا

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


