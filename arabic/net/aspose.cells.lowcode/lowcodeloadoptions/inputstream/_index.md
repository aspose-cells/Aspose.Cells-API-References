---
title: "LowCodeLoadOptions.InputStream"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeLoadOptions. تحصل وتعيّن تدفق القالب"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodeloadoptions/inputstream/
---
## LowCodeLoadOptions.InputStream property

يحصل ويضبط Stream القالب.

```csharp
public Stream InputStream { get; set; }
```

### ملاحظات

عند تعيين تدفق غير null لهذه الخاصية، سيتم تجاهل القيمة التي تم تعيينها مسبقاً لـ [`InputFile`](../inputfile/).

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeLoadOptionsPropertyInputStreamDemo
    {
        public static void Run()
        {
            // إنشاء بيانات تجريبية في تدفق الذاكرة
            byte[] data = { 0x48, 0x65, 0x6C, 0x6C, 0x6F }; // "Hello" in bytes
            using (MemoryStream stream = new MemoryStream(data))
            {
                // إنشاء خيارات تحميل باستخدام InputStream
                var loadOptions = new LowCodeLoadOptions() { InputStream = stream };

                // إنشاء مصنف جديد باستخدام التدفق
                using (Workbook workbook = new Workbook(stream))
                {
                    // الوصول إلى ورقة العمل الأولى
                    Worksheet worksheet = workbook.Worksheets[0];
                    
                    // إظهار أن المحتوى تم تحميله
                    Console.WriteLine("First cell value: " + worksheet.Cells["A1"].Value);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


