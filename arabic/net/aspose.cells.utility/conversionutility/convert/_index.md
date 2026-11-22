---
title: "ConversionUtility.Convert"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ConversionUtility. يحول ملفات Excel إلى صيغ أخرى"
type: docs
url: /ar/net/aspose.cells.utility/conversionutility/convert/
---
## Convert(string, string) {#convert_1}

يقوم بتحويل ملفات Excel إلى صيغ أخرى.

```csharp
public static void Convert(string source, string saveAs)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | String | اسم الملف المصدر. |
| saveAs | String | اسم الملف المتوقع. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ConversionUtilityMethodConvertWithStringStringDemo
    {
        public static void Run()
        {
            // تهيئة مسارات ملفات المصدر والوجهة
            string sourcePath = "source.xlsx";
            string destPath = "output.pdf";
            // تحويل ملف Excel إلى PDF
            ConversionUtility.Convert(sourcePath, destPath);

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## Convert(string, LoadOptions, string, SaveOptions) {#convert}

يقوم بتحويل ملفات Excel إلى صيغ أخرى.

```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs, 
    SaveOptions saveOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | String | اسم الملف المصدر. |
| loadOptions | LoadOptions | خيارات تحميل الملف المصدر. |
| saveAs | String | اسم الملف المتوقع. |
| saveOptions | SaveOptions | خيارات حفظ الملف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ConversionUtilityMethodConvertWithStringLoadOptionsStringSaveOptDemo
    {
        public static void Run()
        {
            // مسارات ملفات المصدر والوجهة
            string sourceFile = "input.csv";
            string outputFile = "output.xlsx";

            // إنشاء ملف CSV تجريبي للتوضيح
            System.IO.File.WriteAllText(sourceFile, "Name,Age\nJohn,30\nAlice,25");

            try
            {
                // إنشاء خيارات التحميل لملف CSV
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                
                // إنشاء خيارات الحفظ لملف XLSX
                SaveOptions saveOptions = new OoxmlSaveOptions();

                // تحويل CSV إلى XLSX باستخدام الخيارات المحددة
                ConversionUtility.Convert(sourceFile, loadOptions, outputFile, saveOptions);

                Console.WriteLine($"File converted successfully from {sourceFile} to {outputFile}");
                
                // تحقق من التحويل بتحميل ملف الإخراج
                Workbook workbook = new Workbook(outputFile);
                Console.WriteLine($"Output file contains {workbook.Worksheets.Count} worksheet(s)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // تنظيف الملفات المؤقتة
                if (System.IO.File.Exists(sourceFile))
                {
                    System.IO.File.Delete(sourceFile);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


