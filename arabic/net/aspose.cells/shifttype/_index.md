---
title: "تعداد ShiftType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ShiftType. يمثل خيارات الإزاحة عند حذف نطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells/shifttype/
---
## ShiftType enumeration

يمثل خيارات الإزاحة عند حذف نطاق من الخلايا.

```csharp
public enum ShiftType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Down | `0` | إزاحة الخلايا إلى الأسفل. |
| Left | `1` | إزاحة الخلايا إلى اليسار. |
| None | `2` | لا تقم بإزاحة الخلايا. |
| Right | `3` | إزاحة الخلايا إلى اليمين. |
| Up | `4` | إزاحة الخلايا إلى الأعلى. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ShiftTypeDemo
    {
        public static void ShiftTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // أدرج صفًا جديدًا عند الفهرس 1، مع إزاحة الصفوف الموجودة إلى الأسفل
            worksheet.Cells.InsertRows(1, 1, true);

            // عيّن قيمة في الصف الذي تم إدراجه حديثًا
            worksheet.Cells["A1"].PutValue("New Item");

            // احذف نطاقًا من الخلايا وحرك الخلايا إلى الأعلى
            worksheet.Cells.DeleteRange(2, 0, 2, 1, ShiftType.Up);

            // أخرج القيم المتبقية في العمود الأول
            for (int row = 0; row < worksheet.Cells.MaxDataRow + 1; row++)
            {
                Console.WriteLine(worksheet.Cells[row, 0].StringValue);
            }

            // احفظ المصنف
            workbook.Save("ShiftTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


