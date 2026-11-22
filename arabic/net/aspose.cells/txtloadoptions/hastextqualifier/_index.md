---
title: "TxtLoadOptions.HasTextQualifier"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. ما إذا كان هناك محدد نص لقيمة الخلية. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/hastextqualifier/
---
## TxtLoadOptions.HasTextQualifier property

ما إذا كان هناك محدد نص لقيمة الخلية. القيمة الافتراضية هي true.

```csharp
public bool HasTextQualifier { get; set; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasTextQualifierDemo
    {
        public static void Run()
        {
            // أنشئ محتوى CSV مع محددات النص
            string csvContent = "\"Name\",\"Age\",\"City\"\n\"John\",30,\"New York\"\n\"Alice\",25,\"London\"";
            
            // احفظ محتوى CSV إلى ملف مؤقت
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvContent, Encoding.UTF8);

            // أنشئ TxtLoadOptions مع تعيين HasTextQualifier إلى true
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // حمّل ملف CSV مع محددات النص
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // احفظ دفتر العمل لإظهار التحميل الناجح
            workbook.Save("Output.xlsx");

            // تنظيف الملف المؤقت
            System.IO.File.Delete(tempFile);
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


