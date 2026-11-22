---
title: "تعداد PrintOrderType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.PrintOrderType تعداد. يمثل ثوابت ترتيب الطباعة"
type: docs
url: /ar/net/aspose.cells/printordertype/
---
## PrintOrderType enumeration

يمثل ثوابت ترتيب الطباعة.

```csharp
public enum PrintOrderType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DownThenOver | `0` | أسفل، ثم يمين |
| OverThenDown | `1` | يمين، ثم أسفل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintOrderTypeDemo
    {
        public static void PrintOrderTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى كائن PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // تعيين ترتيب الطباعة إلى DownThenOver
            pageSetup.Order = PrintOrderType.DownThenOver;

            // تعيين بعض خصائص إعداد الصفحة الأخرى للتوضيح
            pageSetup.PrintArea = "A1:D10";
            pageSetup.PrintTitleRows = "$1:$1";
            pageSetup.PrintTitleColumns = "$A:$A";
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;

            // احفظ المصنف
            workbook.Save("PrintOrderTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


