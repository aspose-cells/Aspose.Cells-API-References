---
title: "AutoFilter.FilterColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFilter. تحصل على مجموعة أعمدة الفلتر"
type: docs
url: /ar/net/aspose.cells/autofilter/filtercolumns/
---
## AutoFilter.FilterColumns property

يحصل على مجموعة أعمدة الفلتر.

```csharp
public FilterColumnCollection FilterColumns { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyFilterColumnsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Status");
            
            worksheet.Cells["A2"].PutValue("HR");
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["C2"].PutValue("Present");
            
            worksheet.Cells["A3"].PutValue("IT");
            worksheet.Cells["B3"].PutValue("Sarah");
            worksheet.Cells["C3"].PutValue("Absent");
            
            worksheet.Cells["A4"].PutValue("HR");
            worksheet.Cells["B4"].PutValue("Mike");
            worksheet.Cells["C4"].PutValue("Present");

            // تطبيق الفلتر التلقائي
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:C1";
            
            // تصفية العمود 2 (Status) للقيم "Present"
            autoFilter.Filter(2, "Present");
            
            // الوصول إلى عمود الفلتر
            FilterColumn filterColumn = autoFilter.FilterColumns[2];
            
            // احفظ المصنف
            workbook.Save("AutoFilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


