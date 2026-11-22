---
title: "AutoFilter.Filter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. تقوم بترشيح قائمة وفقًا لمعايير محددة"
type: docs
url: /ar/net/aspose.cells/autofilter/filter/
---
## AutoFilter.Filter method

يفلتر قائمة بمعايير محددة.

```csharp
public void Filter(int fieldIndex, string criteria)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| معايير | String | المعيار المحدد (سلسلة نصية؛ على سبيل المثال، \"101\"). |

### ملاحظات

ستقوم Aspose.Cells بإزالة جميع إعدادات الفلتر الأخرى على هذا الحقل كما في MS Excel 97-2003.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("Nom1");
            sheet.Cells["A3"].PutValue("Nom2");
            sheet.Cells["A4"].PutValue("Nom3");
            sheet.Cells["A5"].PutValue("Nom2");

            // تطبيق الفلتر التلقائي باستخدام معلمات SetRange الصحيحة
            sheet.AutoFilter.SetRange(0, 0, 4); // startRow: 0, startColumn: 0, endRow: 4
            sheet.AutoFilter.Filter(0, "Nom2"); // Filter column 0 (A) for "Nom2"
            sheet.AutoFilter.Refresh();

            // حفظ النتيجة
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


