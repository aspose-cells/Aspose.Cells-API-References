---
title: "CopyOptions.ReferToDestinationSheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CopyOptions. عند نسخ النطاق في نفس الملف وكان المخطط يشير إلى ورقة المصدر، يعني False أن مصدر بيانات المخطط المنسوخ لن يتغير. يعني True أن مصدر بيانات المخطط المنسوخ يشير إلى ورقة الوجهة."
type: docs
url: /ar/net/aspose.cells/copyoptions/refertodestinationsheet/
---
## CopyOptions.ReferToDestinationSheet property

عند نسخ النطاق في نفس الملف ويشير المخطط إلى ورقة المصدر، يعني False أن مصدر بيانات المخطط المنسوخ لن يتغير. يعني True أن مصدر بيانات المخطط المنسوخ يشير إلى ورقة الوجهة.

```csharp
public bool ReferToDestinationSheet { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false، وتعمل كما في MS Excel. على سبيل المثال: إذا تم نسخ مخطط بمصدر البيانات "sheet1!A1:B10" من ورقة العمل "sheet1" إلى ورقة عمل أخرى "sheet2"، سيتغير مصدر البيانات إلى "sheet2!A1:B10".

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToDestinationSheetDemo
    {
        public static void Run()
        {
            // إنشاء مصنف المصدر مع بيانات عينة
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B1"].PutValue(100);
            sourceSheet.Cells["A2"].PutValue("=SUM(B1)");

            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets.Add("DestinationSheet");

            // تعيين خيارات النسخ باستخدام ReferToDestinationSheet
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ReferToDestinationSheet = true;

            // نسخ ورقة العمل باستخدام الخيارات
            destSheet.Copy(sourceSheet, copyOptions);

            // حفظ النتيجة
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


