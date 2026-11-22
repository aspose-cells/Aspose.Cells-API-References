---
title: "CopyOptions.KeepMacros"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CopyOptions. تشير إلى ما إذا كان سيتم الاحتفاظ بالماكرو"
type: docs
url: /ar/net/aspose.cells/copyoptions/keepmacros/
---
## CopyOptions.KeepMacros property

يشير إلى ما إذا كان يتم الحفاظ على الماكرو؛

```csharp
public bool KeepMacros { get; set; }
```

### ملاحظات

فقط لنسخ المصنف.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyKeepMacrosDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مصدر مع الماكرو (باستخدام ملف قالب يحتوي على ماكرو)
            Workbook srcWorkbook = new Workbook("macros_template.xlsm");
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Macro-enabled source");

            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            
            // تعيين خيارات النسخ مع KeepMacros true
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;

            // نسخ ورقة العمل مع الماكرو
            destWorkbook.Worksheets[0].Copy(srcSheet, options);

            // حفظ النتيجة
            destWorkbook.Save("KeepMacrosExample.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


