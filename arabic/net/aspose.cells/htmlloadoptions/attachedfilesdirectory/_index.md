---
title: "HtmlLoadOptions.AttachedFilesDirectory"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlLoadOptions. الدليل الذي سيتم حفظ الملفات المرفقة فيه"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/attachedfilesdirectory/
---
## HtmlLoadOptions.AttachedFilesDirectory property

الدليل الذي سيتم حفظ الملفات المرفقة فيه.

```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية HtmlLoadOptions.StreamProvider. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2014. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // أنشئ مثيلًا من HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // تحديد الدليل للملفات المرفقة
            options.AttachedFilesDirectory = "C:\\AttachedFiles";

            // تحميل ملف HTML إلى مصنف باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("input.html", options);

            // حفظ المصنف إلى ملف Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


