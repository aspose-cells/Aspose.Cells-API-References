---
title: "TextConverter.Process"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TextConverter. يحول ملف القالب المعطى بين الملفات النصية وغيرها من الصيغ"
type: docs
url: /ar/net/aspose.cells.lowcode/textconverter/process/
---
## Process(string, string) {#process_1}

يقوم بتحويل ملف القالب المحدد بين الملفات النصية والصيغ الأخرى.

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

    public class TextConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            string inputFile = "input.csv";
            string outputFile = "output.xlsx";

            // إنشاء ملف CSV تجريبي
            File.WriteAllText(inputFile, $"Column1,Column2{Environment.NewLine}Data1,Data2{Environment.NewLine}Data3,Data4");

            try
            {
                // استدعِ طريقة Process الساكنة مباشرةً دون إنشاء كائن TextConverter
                TextConverter.Process(inputFile, outputFile);
                
                Console.WriteLine($"Process method successfully converted {inputFile} to {outputFile}");
                Console.WriteLine($"Converted file exists: {File.Exists(outputFile)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
            finally
            {
                // تنظيف الملفات المؤقتة
                if (File.Exists(inputFile))
                {
                    File.Delete(inputFile);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

يقوم بتحويل تنسيق الملف بين الصيغ النصية وصيغ ملفات الجداول الأخرى

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
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class TextConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // أنشئ ملف نصي تجريبي
            string inputText = "Sample text content";
            string inputPath = "input.txt";
            File.WriteAllText(inputPath, inputText);

            // معالجة ملف النص باستخدام خيارات LowCode
            using (FileStream inputStream = new FileStream(inputPath, FileMode.Open))
            {
                TextConverter.Process(
                    new LowCodeLoadOptions() { InputStream = inputStream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.txt"
                    }
                );
            }

            Console.WriteLine("Text processing completed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


