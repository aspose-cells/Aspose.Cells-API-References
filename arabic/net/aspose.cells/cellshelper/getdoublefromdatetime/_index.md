---
title: "CellsHelper.GetDoubleFromDateTime"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. تحويل التاريخ والوقت إلى قيمة مزدوجة"
type: docs
url: /ar/net/aspose.cells/cellshelper/getdoublefromdatetime/
---
## CellsHelper.GetDoubleFromDateTime method

حوّل التاريخ والوقت إلى قيمة مزدوجة.

```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dateTime | DateTime | التاريخ والوقت. |
| date1904 | منطقي | نظام تاريخ 1904. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetDoubleFromDateTimeWithDateTimeBooleanDemo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الحصول على التاريخ والوقت الحاليين
            DateTime now = DateTime.Now;
            
            // تحويل DateTime إلى قيمة مزدوجة باستخدام CellsHelper
            double dateDouble = CellsHelper.GetDoubleFromDateTime(now, false);
            
            // تعيين القيمة في الخلية A1
            worksheet.Cells["A1"].PutValue(dateDouble);
            
            // تنسيق الخلية لعرضها كتاريخ
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Number = 14; // Date format
            worksheet.Cells["A1"].SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("DateTimeConversionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


