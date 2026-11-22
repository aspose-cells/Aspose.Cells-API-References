---
title: "الفئة JsonConverter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.LowCode.JsonConverter. محول لتحويل بنية بيانات json إلى صيغ ملفات جداول أخرى"
type: docs
url: /ar/net/aspose.cells.lowcode/jsonconverter/
---
## JsonConverter class

محول لتحويل بين بنية بيانات json وتنسيقات ملفات الجداول الأخرى.

```csharp
public class JsonConverter
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | يقوم بالتحويل بين بيانات json وصيغ ملفات جداول أخرى. |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process_1)(string, string) | يقوم بتحويل ملف القالب المحدد بين json والصيغ الأخرى. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassJsonConverterDemo
    {
        public static void Run()
        {
            string jsonFilePath = "data.json";
            string excelFilePath = "res.xlsx";

            try
            {
                // تحويل JSON إلى Excel باستخدام Aspose.Cells.LowCode.JsonConverter
                JsonConverter.Process(jsonFilePath, excelFilePath);

                Console.WriteLine("Conversion completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


