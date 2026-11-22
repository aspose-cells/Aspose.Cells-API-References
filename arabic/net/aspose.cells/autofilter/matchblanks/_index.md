---
title: "AutoFilter.MatchBlanks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. مطابقة جميع الخلايا الفارغة في القائمة"
type: docs
url: /ar/net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

مطابقة جميع الخلايا الفارغة في القائمة.

```csharp
public void MatchBlanks(int fieldIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodMatchBlanksWithInt32Demo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات تجريبية مع بعض الخلايا الفارغة
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // اترك C2 فارغًا
            
            worksheet.Cells["A3"].PutValue("Data3");
            // اترك B3 فارغًا
            worksheet.Cells["C3"].PutValue("Data6");
            
            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:C3";
            AutoFilter filter = worksheet.AutoFilter;
            
            // تصفية لإظهار الصفوف فقط التي تحتوي على خلايا فارغة في العمود 3 (C)
            filter.MatchBlanks(2); // Column index is 0-based
            
            // تحديث الفلتر
            filter.Refresh();
            
            // احفظ المصنف
            workbook.Save("AutoFilterMatchBlanksDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


