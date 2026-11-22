---
title: "AutoFilter.FilterTop10"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. تصفية أعلى 10 عناصر في القائمة"
type: docs
url: /ar/net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

تصفية أعلى 10 عناصر في القائمة.

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| isTop | منطقي | يشير إلى ما إذا كان الفلتر من الأعلى أم من الأسفل |
| isPercent | منطقي | يشير إلى ما إذا كانت العناصر نسبة مئوية أم عدد |
| itemCount | Int32 | عدد العناصر |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterTop10WithInt32BooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة (5 صفوف × 3 أعمدة بقيم رقمية)
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Numbers");
            cells["A2"].PutValue(50);
            cells["A3"].PutValue(30);
            cells["A4"].PutValue(80);
            cells["A5"].PutValue(20);
            cells["A6"].PutValue(90);

            // تحديد نطاق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:A6";

            // تطبيق فلتر أعلى 10 (عرض أعلى عنصرين)
            worksheet.AutoFilter.FilterTop10(0, true, false, 2);

            // تحديث الفلتر
            worksheet.AutoFilter.Refresh();

            // احفظ المصنف
            workbook.Save("FilterTop10Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


