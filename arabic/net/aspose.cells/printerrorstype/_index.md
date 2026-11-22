---
title: "تعداد PrintErrorsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.PrintErrorsType. يمثل ثوابت أخطاء الطباعة"
type: docs
url: /ar/net/aspose.cells/printerrorstype/
---
## PrintErrorsType enumeration

يمثل ثوابت أخطاء الطباعة.

```csharp
public enum PrintErrorsType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| PrintErrorsBlank | `0` | يمثل عدم طباعة الأخطاء. |
| PrintErrorsDash | `1` | يمثل طباعة الأخطاء كـ "--". |
| PrintErrorsDisplayed | `2` | يمثل طباعة الأخطاء كما هو معروض. |
| PrintErrorsNA | `3` | يمثل طباعة الأخطاء كـ "#N/A". |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintErrorsTypeDemo
    {
        public static void PrintErrorsTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى PageSetup للورقة
            PageSetup pageSetup = worksheet.PageSetup;

            // تعيين أنواع أخطاء الطباعة المختلفة
            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            workbook.Save("PrintErrorsBlank.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            workbook.Save("PrintErrorsDash.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
            workbook.Save("PrintErrorsDisplayed.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsNA;
            workbook.Save("PrintErrorsNA.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


