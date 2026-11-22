---
title: "JsonConverter.Process"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة JsonConverter. تقوم بتحويل ملف القالب المعطى بين json وصيغ أخرى"
type: docs
url: /ar/net/aspose.cells.lowcode/jsonconverter/process/
---
## Process(string, string) {#process_1}

يقوم بتحويل ملف القالب المحدد بين json والصيغ الأخرى.

```csharp
public static void Process(string templateFile, string resultFile)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| templateFile | String | ملف القالب الذي سيتم تحويله |
| resultFile | String | الملف الناتج |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class JsonConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء بيانات JSON نموذجية وكتابتها إلى ملف مؤقت
            string jsonData = "{\"employees\":[{\"name\":\"John\", \"department\":\"Sales\"}, {\"name\":\"Jane\", \"department\":\"Marketing\"}]}";
            string templatePath = "template.json";
            File.WriteAllText(templatePath, jsonData);

            string resultPath = "output.xlsx";

            try
            {
                // معالجة الملفات مباشرةً باستخدام الطريقة الساكنة لـ JsonConverter
                JsonConverter.Process(templatePath, resultPath);

                Console.WriteLine($"Successfully converted JSON to spreadsheet. Output: {resultPath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Conversion error: {ex.Message}");
            }
            finally
            {
                // تنظيف ملف JSON المؤقت
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

يقوم بالتحويل بين بيانات json وصيغ ملفات جداول أخرى.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | خيارات الإدخال والتحميل |
| saveOptions | LowCodeSaveOptions | خيارات الإخراج والحفظ |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class JsonConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // إنشاء بيانات JSON نموذجية
            string jsonData = "{\"name\":\"John\", \"age\":30, \"city\":\"New York\"}";
            
            // إنشاء تدفق ذاكرة مع بيانات JSON
            using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(jsonData)))
            {
                // معالجة بيانات JSON باستخدام خيارات LowCode
                JsonConverter.Process(
                    new LowCodeLoadOptions() { InputStream = stream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.json"
                    });
            }

            Console.WriteLine("JSON processing completed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


