---
title: "PivotFilter.GetTop10Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotFilter. تحصل على إعداد أعلى 10 للفلتر"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfilter/gettop10value/
---
## PivotFilter.GetTop10Value method

يحصل على إعداد أعلى 10 للمرشح.

```csharp
public Top10Filter GetTop10Value()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetTop10ValueDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى ورقة العمل الأولى وجدول محوري
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // تطبيق فلتر أعلى 10 على الحقل الأساسي الأول (عرض أعلى عنصرين حسب العدد)
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // احصل على الفلتر المطبق وقيمته لأعلى 10
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            Top10Filter top10Filter = filter.GetTop10Value();
            
            // إخراج تفاصيل الفلتر
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Top 10 Items: " + top10Filter.Items);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Top10Filter](../../../aspose.cells/top10filter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


