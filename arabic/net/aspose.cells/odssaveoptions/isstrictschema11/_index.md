---
title: "OdsSaveOptions.IsStrictSchema11"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsSaveOptions. تشير إلى ما إذا كان يجب حفظ ملف ods كإصدار 1.1 من تنسيق ODF. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/odssaveoptions/isstrictschema11/
---
## OdsSaveOptions.IsStrictSchema11 property

تشير إلى ما إذا كان يجب حفظ ملف ods كإصدار 1.1 من تنسيق ODF. القيمة الافتراضية هي false.

```csharp
[Obsolete("Use OdsSaveOptions.OdfStrictVersion property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsStrictSchema11 { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية OdsSaveOptions.OdfStrictVersion. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ فبراير 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyIsStrictSchema11Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample ODS with strict schema");

            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.IsStrictSchema11 = true;
            
            workbook.Save("StrictSchema11Example.ods", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


