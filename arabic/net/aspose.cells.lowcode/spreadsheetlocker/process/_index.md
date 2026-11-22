---
title: "SpreadsheetLocker.Process"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SpreadsheetLocker. تقوم بقفل ملف الجدول باستخدام الإعدادات المحددة"
type: docs
url: /ar/net/aspose.cells.lowcode/spreadsheetlocker/process/
---
## Process(string, string, string, string) {#process_3}

يقفل ملف جدول البيانات بالإعدادات المحددة.

```csharp
public static void Process(string templateFile, string resultFile, string openPassword, 
    string writePassword)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| templateFile | String | ملف القالب الذي سيتم قفله |
| resultFile | String | الملف الناتج |
| openPassword | String | كلمة المرور لتشفير الملف |
| writePassword | String | كلمة المرور لحماية تعديل الجدول |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetLockerMethodProcessWithStringStringStringStringDemo
    {
        public static void Run()
        {           
            string templatePath = "template.xlsx";            
            // تحضير مسار ملف النتيجة
            string resultPath = "secured_spreadsheet.xlsx";

            try
            {
                // تنفيذ طريقة Process باستخدام معلمات نصية مباشرة عبر النوع
                SpreadsheetLocker.Process(
                    templateFile: templatePath,
                    resultFile: resultPath,
                    openPassword: "Open@123",
                    writePassword: "Write@456"
                );

                Console.WriteLine($"Spreadsheet secured successfully. Saved to: {Path.GetFullPath(resultPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error securing spreadsheet: {ex.Message}");
            }
            finally
            {
                // تنظيف القالب المؤقت
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

* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string) {#process_1}

يقفل ملف جدول البيانات بالإعدادات المحددة.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | خيارات الإدخال والتحميل |
| saveOptions | LowCodeSaveOptions | خيارات الإخراج والحفظ |
| openPassword | String | كلمة المرور لتشفير الملف |
| writePassword | String | كلمة المرور لحماية تعديل الجدول |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            
            // معالجة جدول البيانات باستخدام كلمات مرور القفل/فتح القفل
            SpreadsheetLocker.Process(
                new LowCodeLoadOptions() { InputFile = "input.xlsx" },
                new LowCodeSaveOptions() 
                { 
                    OutputFile = "output_locked.xlsx" 
                }, 
                "123456", 
                "234567");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) {#process_2}

يقفل ملف جدول البيانات بالإعدادات المحددة.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword, string workbookPassword, ProtectionType workbookType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | خيارات الإدخال والتحميل |
| saveOptions | LowCodeSaveOptions | خيارات الإخراج والحفظ |
| openPassword | String | كلمة المرور لتشفير الملف |
| writePassword | String | كلمة المرور لحماية تعديل الجدول |
| workbookPassword | String | كلمة المرور لحماية الـ workbook |
| workbookType | ProtectionType | نوع الحماية لحماية الـ workbook |

### انظر أيضًا

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) {#process}

يقفل ملف جدول البيانات بالإعدادات المحددة.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeProtectionProvider provider)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | خيارات الإدخال والتحميل |
| saveOptions | LowCodeSaveOptions | خيارات الإخراج والحفظ |
| provider | AbstractLowCodeProtectionProvider | تنفيذ لتوفير إعدادات الحماية |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
           
            // تحضير LowCodeLoadOptions
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "input.xlsx";

            // تحضير LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            saveOptions.OutputFile = "output.xlsx";

            // إنشاء مزود حماية مخصص
            CustomProtectionProvider provider = new CustomProtectionProvider();

            try
            {
                // استدعاء الطريقة الساكنة Process مع المعلمات المحددة
                SpreadsheetLocker.Process(loadOptions, saveOptions, provider);

                Console.WriteLine("Spreadsheet processed and protected successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error processing spreadsheet: {ex.Message}");
            }

        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override string GetOpenPassword()
            {
                return "open123";
            }

            public override string GetWritePassword()
            {
                return "write123";
            }

            public override string GetWorkbookPassword()
            {
                return "workbook123";
            }

            public override ProtectionType GetWorkbookProtectionType()
            {
                return ProtectionType.All;
            }
        }
    }
}
```

### انظر أيضًا

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeProtectionProvider](../../abstractlowcodeprotectionprovider/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


