---
title: "تعداد AutoFillType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.AutoFillType. يمثل نوع الملء التلقائي"
type: docs
url: /ar/net/aspose.cells/autofilltype/
---
## AutoFillType enumeration

يمثل نوع التعبئة التلقائية.

```csharp
public enum AutoFillType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Copy | `1` | ينسخ القيمة والتنسيق من المنطقة المصدر إلى المنطقة الهدف |
| Default | `0` | يملأ المنطقة الهدف تلقائيًا بالقيمة والتنسيق. |
| Formats | `3` | ينسخ فقط تنسيق المنطقة المصدر إلى المنطقة الهدف. |
| Series | `2` | يمدد القيمة في المنطقة المصدر إلى المنطقة الهدف على شكل سلسلة وينسخ التنسيق إلى المنطقة الهدف. |
| Values | `4` | ينسخ فقط قيمة المنطقة المصدر إلى المنطقة الهدف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFillTypeDemo
    {
        public static void AutoFillTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أنشئ نطاقًا (A1:A10) واملأه ببعض القيم
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A10");
            for (int i = 0; i < 10; i++)
            {
                sourceRange[i, 0].PutValue(i + 1);
            }

            // أنشئ نطاق هدف (B1:B10)
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B10");

            //خطأ نوع السلسلة، تم إنشاء تذكرة
            // استخدم طريقة AutoFill مع AutoFillType.Series لملء النطاق المستهدف
            //sourceRange.AutoFill(targetRange, AutoFillType.Series);

            // استخدم طريقة AutoFill مع AutoFillType.Copy لملء النطاق المستهدف
            sourceRange.AutoFill(targetRange, AutoFillType.Copy);
            // احفظ المصنف
            workbook.Save("AutoFillTypeExample.xlsx");
            workbook.Save("AutoFillTypeExample.pdf");
        }
    }

}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


