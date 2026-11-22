---
title: "الفئة LowCodeLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.LowCode.LowCodeLoadOptions. خيارات تحميل ملف القالب"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodeloadoptions/
---
## LowCodeLoadOptions class

خيارات تحميل ملف القالب.

```csharp
public class LowCodeLoadOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | يحصل ويضبط ملف (مع المسار إذا لزم) القالب. |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | يحصل ويضبط Stream القالب. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            // إنشاء Stream عيني (في الذاكرة لأغراض العرض)
            using (MemoryStream stream = new MemoryStream())
            {
                // إنشاء مصنف جديد وحفظه إلى Stream للعرض
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Save(stream, SaveFormat.Xlsx);

                // إعادة تعيين موضع Stream
                stream.Position = 0;

                // إنشاء واستخدام LowCodeLoadOptions
                var loadOptions = new LowCodeLoadOptions()
                {
                    InputStream = stream
                };

                // مثال على الاستخدام - عادةً ما يتم تمريره إلى طريقة معالجة
                Console.WriteLine($"Loading with LowCode options from stream of length: {loadOptions.InputStream.Length}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


