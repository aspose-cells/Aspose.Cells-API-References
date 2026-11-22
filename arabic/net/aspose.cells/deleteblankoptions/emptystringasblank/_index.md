---
title: "DeleteBlankOptions.EmptyStringAsBlank"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DeleteBlankOptions. تشير إلى ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون قيمتها سلسلة فارغة. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/deleteblankoptions/emptystringasblank/
---
## DeleteBlankOptions.EmptyStringAsBlank property

يشير إلى ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون قيمتها سلسلة فارغة. القيمة الافتراضية هي true.

```csharp
public bool EmptyStringAsBlank { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyStringAsBlankDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء ورقة العمل بالبيانات بما في ذلك السلاسل الفارغة
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // تكوين DeleteBlankOptions مع EmptyStringAsBlank مضبوطة على true
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true
            };

            // حذف الصفوف التي تحتوي على سلاسل فارغة (تُعامل كفراغات)
            worksheet.Cells.DeleteBlankRows(options);

            // حفظ النتيجة
            workbook.Save("DeleteBlankOptions_EmptyStringAsBlank_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


