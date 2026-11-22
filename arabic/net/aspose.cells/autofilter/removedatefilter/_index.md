---
title: "AutoFilter.RemoveDateFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. تزيل فلتر التاريخ"
type: docs
url: /ar/net/aspose.cells/autofilter/removedatefilter/
---
## AutoFilter.RemoveDateFilter method

يزيل مرشح تاريخ.

```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| dateTimeGroupingType | DateTimeGroupingType | نوع التجميع |
| سنة | Int32 | السنة. |
| شهر | Int32 | الشهر. |
| يوم | Int32 | اليوم. |
| ساعة | Int32 | الساعة. |
| دقيقة | Int32 | الدقيقة. |
| ثانية | Int32 | الثانية. |

### ملاحظات

إذا كان DateTimeGroupingType هو Year، فإن معلمة السنة فقط هي المؤثرة. إذا كان DateTiemGroupingType هو Month، فإن معلمتي السنة والشهر فقط هما المؤثرتين.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveDateFilterWithInt32DateTimeGroupingTypeInt32Demo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // إضافة بيانات عينة مع تواريخ
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue(new DateTime(2020, 1, 7));
            sheet.Cells["A3"].PutValue(new DateTime(2020, 1, 8));
            sheet.Cells["A4"].PutValue(new DateTime(2020, 1, 9));
            
            // تطبيق الفلتر التلقائي
            sheet.AutoFilter.Range = "A1:A4";
            
            // إضافة مرشح تاريخ لليوم 7
            sheet.AutoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // تحقق من تطبيق المرشح
            Console.WriteLine("Row 2 hidden: " + sheet.Cells.IsRowHidden(1)); // Should be true
            
            // إزالة مرشح التاريخ
            sheet.AutoFilter.RemoveDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // تحقق من إزالة المرشح
            Console.WriteLine("Row 2 hidden after removal: " + sheet.Cells.IsRowHidden(1)); // Should be false
        }
    }
}
```

### انظر أيضًا

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


