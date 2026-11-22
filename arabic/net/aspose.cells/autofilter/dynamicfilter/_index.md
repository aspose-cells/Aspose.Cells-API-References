---
title: "AutoFilter.DynamicFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. تضيف مرشحًا ديناميكيًا"
type: docs
url: /ar/net/aspose.cells/autofilter/dynamicfilter/
---
## AutoFilter.DynamicFilter method

يضيف مرشحًا ديناميكيًا.

```csharp
public void DynamicFilter(int fieldIndex, DynamicFilterType dynamicFilterType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| dynamicFilterType | DynamicFilterType | نوع الفلتر الديناميكي. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodDynamicFilterWithInt32DynamicFilterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            // تطبيق الفلتر التلقائي باستخدام توقيع الطريقة الصحيح
            worksheet.AutoFilter.Range = "A1:A6";

            // طبق مرشحًا ديناميكيًا لتواريخ مارس
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            workbook.Save("DynamicFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


