---
title: "الفئة CopyOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CopyOptions. تمثل خيارات النسخ"
type: docs
url: /ar/net/aspose.cells/copyoptions/
---
## CopyOptions class

يمثل خيارات النسخ.

```csharp
public class CopyOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CopyOptions](copyoptions/)() | منشئ CopyOptions. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ColumnCharacterWidth](../../aspose.cells/copyoptions/columncharacterwidth/) { get; set; } | يشير إلى ما إذا كان يتم نسخ عرض العمود بوحدة الأحرف. |
| [CopyInvalidFormulasAsValues](../../aspose.cells/copyoptions/copyinvalidformulasasvalues/) { get; set; } | إذا كانت الصيغة غير صالحة للوجهة المستهدفة، يتم نسخ القيم فقط. |
| [CopyNames](../../aspose.cells/copyoptions/copynames/) { get; set; } | يشير إلى ما إذا كان يتم نسخ الأسماء. |
| [ExtendToAdjacentRange](../../aspose.cells/copyoptions/extendtoadjacentrange/) { get; set; } | يشير إلى ما إذا كان يتم توسيع النطاقات عند نسخ النطاق إلى نطاق مجاور. |
| [KeepMacros](../../aspose.cells/copyoptions/keepmacros/) { get; set; } | يشير إلى ما إذا كان يتم الحفاظ على الماكرو؛ |
| [ReferToDestinationSheet](../../aspose.cells/copyoptions/refertodestinationsheet/) { get; set; } | عند نسخ النطاق في نفس الملف ويشير المخطط إلى ورقة المصدر، يعني False أن مصدر بيانات المخطط المنسوخ لن يتغير. يعني True أن مصدر بيانات المخطط المنسوخ يشير إلى ورقة الوجهة. |
| [ReferToSheetWithSameName](../../aspose.cells/copyoptions/refertosheetwithsamename/) { get; set; } | في مايكروسوفت إكسل، عند نسخ الصيغ التي تشير إلى أوراق عمل أخرى أثناء نسخ ورقة عمل إلى أخرى، يجب أن تشير الصيغ المنسوخة إلى مصنف المصدر. ومع ذلك، في بعض الحالات قد يحتاج المستخدم إلى أن تشير الصيغ المنسوخة إلى أوراق عمل ذات الاسم نفسه في نفس المصنف، مثل عندما تكون تلك الأوراق قد تم نسخها قبل عملية النسخ هذه، لذا يجب الحفاظ على هذه الخاصية كقيمة true. |
| [UpdateInvalidReferencesToTargetSheet](../../aspose.cells/copyoptions/updateinvalidreferencestotargetsheet/) { get; set; } | يشير إلى ما إذا كان يجب الإشارة إلى ورقة العمل الهدف إذا لم يتم نسخ ورقة العمل المشار إليها. |

### أمثلة

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CopyOptionsDemo
    {
        public static void CopyOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // إنشاء دفتر عمل جديد لنسخ البيانات إليه
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // إنشاء كائن CopyOptions
            CopyOptions copyOptions = new CopyOptions
            {
                KeepMacros = true,
                ExtendToAdjacentRange = true,
                CopyNames = true,
                CopyInvalidFormulasAsValues = true,
                ColumnCharacterWidth = true,
                ReferToSheetWithSameName = true,
                ReferToDestinationSheet = true
            };

            // نسخ البيانات من ورقة العمل المصدر إلى ورقة العمل الوجهة
            destSheet.Cells.CopyRows(sheet.Cells, 0, 0, 2, copyOptions);

            // حفظ دفتر العمل الوجهة
            destWorkbook.Save("CopyOptionsExample.xlsx");
            destWorkbook.Save("CopyOptionsExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


